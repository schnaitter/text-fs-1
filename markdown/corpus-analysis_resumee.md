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

In diesem Kapitel wurde durch eine quantitative Analyse von Worthäufigkeiten des semantischen Felds "Grippe" die Forschungsfrage untersucht, ob sich für die Spanische Grippe 1918/1919 mit Fokus auf den Berliner Raum Muster in der öffentlichen Aufmerksamkeit ausmachen lassen, die eine wellenartige Verlaufsform aufweisen. Dafür wurde vorgestellt, wie die Häufigkeitsanalyse auf einem annotierten Korpus durchgeführt und visualisiert werden können. Um die Textstellen genauer betrachten zu können, die sich mit der Grippe auseinandersetzen, wurde die Key Word in context (KWIC)-Darstellung eingeführt. 
Durch die Häufigkeitsanalyse konnte gezeigt, dass die Aufmerksamkeit auf die Spanische Grippe Wellen schlägt. Die Minima und Maxima stimmen dabei mit denen der Grippewellen überein.

## Lernstandskontrolle

Dummy-Quiz:
```{code-cell} ipython3
:tags: [remove-input]
display_quiz("../assessment/ocr_quizzes.json", colors = colors.jupyterquiz)
```