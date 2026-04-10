---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "Virtually Free: Making Strict IO Memory Protection Feasible for Virtualized Environments"
authors: [Leshna Balara,
          admin,
          Ishvik Kumar Singh,
          Owen Jack Cochell,
          Jiyuan Zhang,
          Rachit Agarwal,
          Tianyin Xu,
          Saksham Agarwal (* denotes equal contribution)
]
author_notes: ["Equal contribution", "Equal contribution"]
date: "2026-04-10"
doi: ""

# Schedule page publish date (NOT publication's date).
publishDate: "2026-04-10T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["3"]

# Publication name and optional abbreviated publication name.
publication: "In Submission"
publication_short: "In Submission"

abstract: "IO memory protection prevents malicious DMA-capable IO devices from executing errant data transfers into host memory. Modern servers enable memory protection by requiring IO devices to operate on virtual IO addresses, and using IOMMU to perform fast virtual-to-physical address translation upon each DMA. Existing IO memory protection mechanisms offers powerful, so-called strict, safety guarantees; however, they require at least one VM exit per DMA in virtualized environments to invalidate translation entries in IOMMU caches. These VM exits in strict protection---even with state-of-the-art device passthrough mechanisms, memory management, and hardware-assisted translation---result in 83--95% degradation in application-level throughput! Real-world deployments today have to choose either high performance or strict IO memory protection, but not both.

We present vFree, a simple modification to existing IO memory protection mechanisms that makes strict IO memory protection feasible in virtualized environments. The key insight in vFree is that, in virtualized environments, it is possible to reduce the overheads of strict IO memory protection to a bare minimum by increasing the cost of address translation. Intuitively, this is because each VM exit has much higher cost than the worst-case translation cost. vFree design incorporates two ideas---one-for-many invalidations and deferred free page---that, when put together, result in higher address translation cost but significantly reduce the number of VM exits (and hence, IO memory protection overheads) while maintaining strict IO memory protection. We implement vFree on Linux, and evaluate it across multiple real-world applications. Our evaluation suggests that, at the cost of one dedicated core, vFree consistently achieves performance within 1-8% of the unprotected system---74-147× higher than state-of-the-art IO memory protection mechanisms."

# Summary. An optional shortened abstract.
summary: "A simple modification to IO memory protection that makes strict protection feasible in virtualized environments, achieving performance close to unprotected systems"

tags: [Operating Systems, Memory System]
categories: [Operating System]
featured: true

# Custom links (optional).
#   Uncomment and edit lines below to show custom links.
links:
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