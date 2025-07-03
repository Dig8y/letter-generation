# AI Letter Generation Pipeline Overview

https://www.loom.com/share/d0623f43552a496191a319838d60f79f

## 1. End-to-End Workflow


1. **Draft**  
   • `draft_letter()` merges general + specific templates with case content and calls Gemini.

2. **Evaluate** *(core evaluation stack)*  
   • Two modes  
     a. *Simple* – direct audit prompt.  
     b. *Enhanced* – fact extraction → fact verification → score comptrilation.  
   • Structured outputs parsed by Pydantic models.

3. **Human Review**  
   • CLI prompts guide accept / AI-improve / manual-improve decisions.  
   • Each iteration is persisted under `sessions/`.

4. **Template Evolution**  
   • Templates saved per iteration; diff & export utilities included.

---

## 2. Evaluation Pipeline Deep-Dive

| Stage | Technique | Comments |
|-------|-----------|----------|
| Extract **case facts** | Gemini JSON mode (`CaseFactsResponse`) | One-time per session (cached). |
| Extract **letter facts** | Gemini JSON mode (`LetterFactsResponse`) | Capped at just for time |
| **Verify** facts | For each letter fact, compare against case facts with structured verdict (`FactVerificationResult`). | Serial calls (rate-limited). |
| **Compile** results | Aggregate verdicts → hallucination list + score → decide which template needs improvement. | Threshold: pass if ≥95 % supported. |

**Strengths**  
• Granular hallucination types (fabricated, unsupported, factual error, inconsistency).  
• Structured outputs reduce parsing fragility.  
• Session-level caching of case facts saves cost.

---

## How to Run (Quick Start)

```bash
# 1. Install
python -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt

# 2. Configure
echo "GOOGLE_API_KEY=sk-..." > .env
# optional: export MODEL=gemini-2.5-flash

# 3. Launch interactive session
jupyter notebook ai_letter_pipeline.ipynb   # run Cell 8
```
