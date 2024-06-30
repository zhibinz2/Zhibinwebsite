---
title: "Detecting the state of drowsiness induced by propofol by spatial filter and machine learning algorithm on EEG recording"
authors:
- Zhibin Zhou
- Ramesh Srinivasan
author_notes:
- "Equal contribution"
- "Equal contribution"
date: "2021-07-01T00:00:00Z"
doi: ""

# Schedule page publish date (NOT publication's date).
publishDate: "2021-07-01T00:00:00Z"

# Publication type.
# Accepts a single type but formatted as a YAML list (for Hugo requirements).
# Enter a publication type from the CSL standard.
publication_types: ["journal article"]

# Publication name and optional abbreviated publication name.
publication: "*Journal of Source Themes, 1*(1)"
publication_short: ""

abstract: To accurately measure the depth of anesthesia has been a challenge for both anesthesiologists and engineers who work on developing tools of measurements. This study aims to use a machine-learning algorithm to predict the drowsy state, a transitional depth of sedation during propofol anesthesia. The data used in this study were scalp EEG (electroencephalogram) recordings selected from the University of Cambridge Repository. Raw EEG recordings were preprocessed into power spectrum matrices one second per sample. A total of 170 samples (110 awake samples and 60 drowsy samples) were used. A CNN (Convolutional Neural Network) for the MNIST (Modified National Institute of Standards and Technology) dataset was applied on these EEG power spectrum matrices. Due to the small dataset volume, Leave-One-Out cross-validation was used to train the data. Results of the training accuracy reached 99.69%. And test accuracy averaged 96.47%. Overall, the model is able to predict the state of drowsiness during propofol anesthesia. This provides the potential to develop EEG monitoring devices with closed-loop feedback of such a machine learning algorithm that controls the titration of the dosage of anesthetic administration and the depth of anesthesia.

# Summary. An optional shortened abstract.
summary: A paradigm such as this can be applied in clinical EEG monitoring in real-time, guiding anesthesiologists and critical care physicians to determine the optimal dosage of anesthetic for small diagnostic and surgical procedures.

tags:
- Source Themes
featured: false

# links:
# - name: ""
#   url: ""
url_pdf: https://www.biorxiv.org/content/10.1101/2021.07.12.452077v1.full.pdf
url_code: 'https://github.com/HugoBlox/hugo-blox-builder'
url_dataset: ''
url_poster: ''
url_project: ''
url_slides: ''
url_source: ''
url_video: ''

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
image:
  caption: 'Image credit: [**Unsplash**](https://unsplash.com/photos/jdD8gXaTZsc)'
  focal_point: ""
  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
projects: []

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
slides: example
---

{{% callout note %}}
Click the *Cite* button above to demo the feature to enable visitors to import publication metadata into their reference management software.
{{% /callout %}}

{{% callout note %}}
Create your slides in Markdown - click the *Slides* button to check out the example.
{{% /callout %}}

Add the publication's **full text** or **supplementary notes** here. You can use rich formatting such as including [code, math, and images](https://docs.hugoblox.com/content/writing-markdown-latex/).
