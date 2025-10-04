---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "EMT: An OS Framework for New Memory Translation Architectures"
authors: [admin,
          Jiyuan Zhang,
          Jongyul Kim,
          Alan Wang,
          Fan Chung,
          Jovan Stojkovic,
          Weiwei Jia,
          Dimitrios Skarlatos,
          Josep Torrellas,
          Tianyin Xu
]
date: "2025-04-27"
doi: ""

# Schedule page publish date (NOT publication's date).
publishDate: "2025-07-05T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["1"]

# Publication name and optional abbreviated publication name.
publication: "Operating Systems Design and Implementation"
publication_short: "OSDI"

abstract: "With terabyte-scale memory capacity and memory-intensive workloads, memory translation has become a major performance bottleneck. Many novel hardware schemes are developed to speed up memory translation, but few are experimented with commodity OSes. A main reason is that memory management in major OSes, like Linux, does not have the extensibility to empower emerging hardware schemes.

We develop EMT, a pragmatic framework atop Linux to empower different hardware schemes of memory translation such as radix tree and hash table. EMT provides an architecture neutral interface that 1) supports diverse memory translation architectures, 2) enables hardware-specific optimizations, 3) accommodates modern hardware and OS complexity, and 4) has negligible overhead over hardwired implementations. We port Linux’s memory management onto EMT and show that EMT enables extensibility without sacrificing performance. We use EMT to implement OS support for ECPT and FPT, two recent experimental translation schemes for fast translation; EMT enables us to understand the OS perspective of these architectures and further optimize their designs."

# DeepCOVID-XR is an artificial intelligence algorithm for detecting COVID-19 on chest X-rays,trainedandtested on the largest published clinical dataset in the COVID-19 era with performance similarto the consensus of experienced, cardiothoracic fellowship-trainedthoracic radiologists. We present DeepCOVID-XR, a deep learning AI algorithm for detecting CXRs suspicious for COVID-19, trained and tested on the largest published clinical dataset from the COVID-19 era to date. 

# Summary. An optional shortened abstract.
summary: "Designed a hardware-neutral, extensible framework with minimal overhead that supports diverse memory translation schemes."

# DeepCOVID-XR is an deep learning algorithm for detecting COVID-19 on chest X-rays,trained and tested on the largest published clinical dataset in the COVID-19 era with performance similar to the consensus of experienced, cardiothoracic fellowship-trained thoracic radiologists.
tags: [Operating systems, memory systems]
categories: [Operating System]
featured: true

# Custom links (optional).
#   Uncomment and edit lines below to show custom links.
links:
url_pdf: files/publications/emt.pdf
url_code: https://github.com/xlab-uiuc/emt
url_dataset:
url_poster:
url_project:
url_slides: https://github.com/xlab-uiuc/emt/blob/main/EMT-OSDI.pptx
url_source: 
url_video: https://www.usenix.org/conference/osdi25/presentation/chai-siyuan
# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: ""
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
slides: ""
---
