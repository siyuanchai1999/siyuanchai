---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "KARAT: Kernel Implementation of Compiler-and Runtime-Based Address Translation"
authors: [
    Working With
    Brian Suchy, 
    Souradip Ghosh, 
    Drew Kersnar, 
    Zhen Huang,
    Simone Campanoni, 
    Peter Dinda
    (Target to Sumbit in DEC 2020 for OSDI)
]
date: "2020-12-15"
doi: ""

# Schedule page publish date (NOT publication's date).
publishDate: "2020-10-01T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["3"]

# Publication name and optional abbreviated publication name.
publication: "USENIX Symposium on Operating Systems Design and Implementation"
publication_short: "OSDI"

abstract: "In modern operating system, virtual and physical address translation is done through paging. We argue that different address space implementations could be more competitive than paging. Within an experimental aero-kernel, Nautilus, we decouple the abstraction of address spaces from its implementation and implement paging as well as a new novel implementation, KARAT, which is an allocation level address space implementation based on Compiler-and Runtime-Based Address Translation (CARAT). Using KARAT, we show that the same functionality of paging is possible while providing new benefits such as finer grain control of memory. KARAT is implemented using a combination of the kernel, compiler, and runtime which operates without needing to make changes to the original code. 
"

# DeepCOVID-XR is an artificial intelligence algorithm for detecting COVID-19 on chest X-rays,trainedandtested on the largest published clinical dataset in the COVID-19 era with performance similarto the consensus of experienced, cardiothoracic fellowship-trainedthoracic radiologists. We present DeepCOVID-XR, a deep learning AI algorithm for detecting CXRs suspicious for COVID-19, trained and tested on the largest published clinical dataset from the COVID-19 era to date. 

# Summary. An optional shortened abstract.
summary: "Use compiler and Runtime in kernel to replace paging for virtual address translation"

# DeepCOVID-XR is an deep learning algorithm for detecting COVID-19 on chest X-rays,trained and tested on the largest published clinical dataset in the COVID-19 era with performance similar to the consensus of experienced, cardiothoracic fellowship-trained thoracic radiologists.
tags: [Memory, Compiler, Runtime]
categories: [Operating System]
featured: true

# Custom links (optional).
#   Uncomment and edit lines below to show custom links.
# links:
# - name: Follow
#   url: https://twitter.com
#   icon_pack: fab
#   icon: twitter

url_pdf:
url_code:
url_dataset:
url_poster:
url_project:
url_slides:
url_source:
url_video:

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
