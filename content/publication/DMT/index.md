---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "Direct Memory Translation for Virtualized Clouds"
authors: [Jiyuan Zhang,
          Weiwei Jia,
          admin,
          Peizhe Liu,
          Jongyul Kim, 
          Tianyin Xu
]
date: "2024-04-27"
doi: ""

# Schedule page publish date (NOT publication's date).
publishDate: "2024-04-27T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["1"]

# Publication name and optional abbreviated publication name.
publication: "Architectural Support for Programming Languages and Operating Systems"
publication_short: "ASPLOS"

abstract: "Virtual memory translation has become a key performance bottleneck of memory-intensive workloads in virtualized cloud environments. On the x86 architecture, a nested translation needs to sequentially fetch up to 24 page table entries (PTEs). This paper presents Direct Memory Translation (DMT), a hardware-software extension for x86-based virtual memory that minimizes translation overhead while maintaining backward compatibility with x86. In DMT, the OS manages last-level PTEs in a contiguous physical memory region, termed Translation Entry Areas (TEAs). DMT establishes a direct mapping from each virtual page in a Virtual Memory Area (VMA) to the corresponding PTE in a TEA. Since processes manage memory with a handful of major VMAs, the mapping can be maintained per VMA and effectively stored in a few dedicated registers. DMT further optimizes virtualized memory translation via guest-host cooperation by directly allocating guest TEAs in physical memory, bypassing intermediate virtualization layers. DMT is inherently scalable---it takes one, two, and three memory references in native, virtualized, and nested virtualized setups. Its scalability enables hardware-assisted translation for nested virtualization. Our evaluation shows that DMT significantly speeds up page walks by an average of 1.58x (1.65x with THP) in a virtualized setup, resulting in 1.20x (1.14x with THP) speedup of application execution on average."

# DeepCOVID-XR is an artificial intelligence algorithm for detecting COVID-19 on chest X-rays,trainedandtested on the largest published clinical dataset in the COVID-19 era with performance similarto the consensus of experienced, cardiothoracic fellowship-trainedthoracic radiologists. We present DeepCOVID-XR, a deep learning AI algorithm for detecting CXRs suspicious for COVID-19, trained and tested on the largest published clinical dataset from the COVID-19 era to date. 

# Summary. An optional shortened abstract.
summary: "Directly fecthing last level PTEs to accelerate virtual to physical address translation"

# DeepCOVID-XR is an deep learning algorithm for detecting COVID-19 on chest X-rays,trained and tested on the largest published clinical dataset in the COVID-19 era with performance similar to the consensus of experienced, cardiothoracic fellowship-trained thoracic radiologists.
tags: [Operating systems, Memory system]
categories: [Memory system]
featured: true

# Custom links (optional).
#   Uncomment and edit lines below to show custom links.
links:
- name: "ASPLOS"
  url: https://dl.acm.org/doi/10.1145/3620665.3640358
  icon_pack: fab

url_pdf: files/publications/dmt.pdf
url_code: https://github.com/xlab-uiuc/dmt
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
