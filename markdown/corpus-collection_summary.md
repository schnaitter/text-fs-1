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
In diesem Kapitel haben wir uns zunächst über unterschiedliche [Typen von Korpora bzw. Strategien der Korpusbildung](corpus-collection_corpora-as-research-objects) in den Digital Humanities verständigt, um danach eine differenzierte Vorstellung von den u[nterschiedlichen Erscheinungsformen und Formaten von "Text" im digitalen Raum ](corpus-collection_text_as_digital_objects)zu entwickeln. Wir haben des Weiteren eine Idee von der [Funktion und der Struktur von Metadaten für die Korpusbeschreibung](corpus-collection_metadata) entwickelt und diese dann – sowohl auf Ebene des Gesamtkorpus als auch auf Ebene der einzelnen Korpuselemente – auf unser Forschungskorpus angewandt. Schließlich haben wir das mit Metadaten hinreichend beschriebene [Forschungskorpus durch einen automatisierten Download aufgebaut](corpus-collection_building-our-corpus). Damit ist unser Forschungskorpus fertig und kann in den nächsten Schritten aufbereitet und angereichert werden. 

## Lernstandskontrolle

Dummy-Quiz:
```{code-cell} ipython3
:tags: [remove-input]
display_quiz("../assessment/ocr_quizzes.json", colors = colors.jupyterquiz)
```