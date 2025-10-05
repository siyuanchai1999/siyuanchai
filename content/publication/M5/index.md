---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "M5: Mastering Page Migration and Memory Management for CXL-based Tiered Memory system"
authors: [Yan Sun, Jongyul Kim, Zeduo Yu, Jiyuan Zhang, admin, Michael Jaemin Kim, Hwayong Nam, Jaehyun Park, Eojin Na, Yifan Yuan, Ren Wang, Jung Ho Ahn, Tianyin Xu, Nam Sung Kim
]
date: "2025-03-30"
doi: ""

# Schedule page publish date (NOT publication's date).
publishDate: "2025-03-30T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["1"]

# Publication name and optional abbreviated publication name.
publication: "Architectural Support for Programming Languages and Operating Systems"
publication_short: "ASPLOS"

abstract: "CXL has emerged as a promising memory interface that can
cost-effectively expand the capacity and bandwidth of a memory system, complementing the traditional DDR interface.
However, CXL DRAM presents 2–3× longer access latency
than DDR DRAM, forming a tiered-memory system that demands an effective and efficient page-migration solution. Although many page-migration solutions have been proposed
for past tiered-Memory system, they have achieved limited
success. To tackle the challenge of managing tiered-memory
systems, this work first presents a CXL-driven profiling solution to precisely and transparently count the number of
accesses to every 4KB page and 64B word in CXL DRAM.
Second, using the profiling solution, this work uncovers that
(1) widely used CPU-driven page-migration solutions often
identify warm pages as hot pages, and (2) certain applications have sparse hot pages, where only a small percentage
of words in each of these pages are frequently accessed.

Besides, this work demonstrates that the performance overhead of identifying hot pages is sometimes high enough to
degrade application performance. Lastly, this work presents
M5, a platform designed to facilitate the development of
effective CXL-driven page-migration solutions, providing
hardware-based hot-page and hot-word trackers in the CXL
controller. On average, M5 can identify 47% hotter pages
and offer 14% higher performance than the best CPU-driven
page-migration solution, even with a simple policy.
"

# DeepCOVID-XR is an artificial intelligence algorithm for detecting COVID-19 on chest X-rays,trainedandtested on the largest published clinical dataset in the COVID-19 era with performance similarto the consensus of experienced, cardiothoracic fellowship-trainedthoracic radiologists. We present DeepCOVID-XR, a deep learning AI algorithm for detecting CXRs suspicious for COVID-19, trained and tested on the largest published clinical dataset from the COVID-19 era to date. 

# Summary. An optional shortened abstract.
summary: "Developed a CXL-driven hot-page and hot-word profiling solution"

# DeepCOVID-XR is an deep learning algorithm for detecting COVID-19 on chest X-rays,trained and tested on the largest published clinical dataset in the COVID-19 era with performance similar to the consensus of experienced, cardiothoracic fellowship-trained thoracic radiologists.
tags: [Operating systems, Memory system]
categories: [Memory system]
featured: true

# Custom links (optional).
#   Uncomment and edit lines below to show custom links.
links:
- name: "ASPLOS"
  url: https://dl.acm.org/doi/10.1145/3676641.3711999
  icon_pack: fab

url_pdf: files/publications/m5.pdf
url_code: https://github.com/ece-fast-lab/ASPLOS-2025-M5
url_dataset: 
url_poster:
url_project:
url_slides: files/publications/m5.pptx
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
