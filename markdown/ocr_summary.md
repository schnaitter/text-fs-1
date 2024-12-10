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

Dieses Kapitel führte [OCR](ocr) als Methode zur maschinellen Lesbarkeit Ihres Korpus ein. Es zeigte, wie [OCR in Python](../data-input/FS_1_MVP_OCR) durchgeführt werden kann und wie die [Qualität der OCR](ocr-quality) bewertet werden kann. Das nächste Kapitel wird sich der Nachkorrektur der OCR-Ergebnisse widmen.

## Lernstandskontrolle

Dummy-Quiz:
```{code-cell} ipython3
:tags: [remove-input]
display_quiz("../assessment/ocr_quizzes.json", colors = colors.jupyterquiz)
```