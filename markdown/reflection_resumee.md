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
# Abschließende Lernstandskontrolle

Dummy-Quiz:
```{code-cell} ipython3
:tags: [remove-input]
display_quiz("../assessment/ocr_quizzes.json", colors = colors.jupyterquiz)
```