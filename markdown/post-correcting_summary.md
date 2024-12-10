---
jupytext:
  formats: md:myst
  text_representation:
    extension: .md
    format_name: myst
kernelspec:
  display_name: Python 3
  language: python
  name: python3
---
```{code-cell} ipython3
:tags: [remove-cell]
from jupyterquiz import display_quiz
import sys
sys.path.append("..")
from quadriga_config import colors
```

# Resümee

Dieses Kapitel demonstrierte, wie die Ergebnisse von OCR [nachbearbeitet](post-correcting_ocr) werden können. Es führte [regelbasierte Nachkorrektur](data-input/FS_1_MVP_Post_Correcting_OCR) mit regulären Ausdrücken (in Python) ein und gab einen Einblick in die Möglichkeiten der [LLM-basierten Nachkorrektur](post-correcting_llm). Im nächsten Kapitel werden die nachkorrigierten Ergebnisse von OCR weiter mit NLP-Methoden verarbeitet.

## Lernstandskontrolle

Dummy-Quiz:
```{code-cell} ipython3
:tags: [remove-input]
display_quiz("../assessment/ocr_quizzes.json", colors = colors.jupyterquiz)
```