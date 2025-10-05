---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "CARAT CAKE: Replacing Paging via Compiler/Kernel Cooperation"
authors: [
    Brian Suchy,
    Souradip Ghosh,
    Drew Kersnar,
    admin,
    Zhen Huang,
    Aaron Nelson,
    Michael Cuevas,
    Alex Bernat,
    Gaurav Chaudhary,
    Nikos Hardavellas,
    Simone Campanoni,
    Peter Dinda,
]
date: "2022-02-11"
doi: ""

# Schedule page publish date (NOT publication's date).
publishDate: "2020-10-01T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["1"]

publication_short: "ASPLOS"

# Publication name and optional abbreviated publication name.
# publication: "USENIX Symposium on Operating Systems Design and Implementation"
# publication_short: "OSDI"
publication: ""
abstract: "Virtual memory, specifically paging, is currently being challenged by new demands from modern workloads and this challenge is driving innovation in hardware/software codesign. Recent work has demonstrated the potential of an alternative software/software codesign, in which the combination of the compiler and kernel achieves the goals of virtual memory for unmanaged languages. This design can result in dramatically simplified hardware requirements, even to the point of supporting only physical addressing. This freedom in turn provides enhanced freedom for cache design, which is currently coupled with address translation. While the case for this Compiler- And Runtime-based Address Translation (CARAT) concept has been made, the previous evaluation was based on a user-level prototype and did not address the numerous challenges posed by kernel-level implementation of abstractions such as processes on top of CARAT. This work demonstrates that these challenges can be surmounted.

We report on incorporating CARAT into a kernel, forming Compiler- And Runtime-based Address Translation for CollAborative Kernel Environments (CARAT CAKE). In our prototype implementation, a Linux-compatible x64 process abstraction can be based either on CARAT CAKE, or on a sophisticated paging implementation. Implementing CARAT CAKE involves not only kernel changes, but also new compiler optimizations and transformations that must work on all code in the system, including kernel code. We evaluate our CARAT CAKE implementation in comparison with paging (and with traditional Linux) using the NAS benchmark suite. We find that CARAT CAKE is able to achieve the protection, mapping, and movement properties of paging as well as the ability to move and compact both user and kernel memory, as required by physical addressing, with reasonable overhead. However, CARAT CAKE’s memory management can operate at arbitrary granularity instead of being restricted to pages and the hardware is not involved in memory management.
"

# DeepCOVID-XR is an artificial intelligence algorithm for detecting COVID-19 on chest X-rays,trainedandtested on the largest published clinical dataset in the COVID-19 era with performance similarto the consensus of experienced, cardiothoracic fellowship-trainedthoracic radiologists. We present DeepCOVID-XR, a deep learning AI algorithm for detecting CXRs suspicious for COVID-19, trained and tested on the largest published clinical dataset from the COVID-19 era to date. 

# Summary. An optional shortened abstract.
summary: "Use compiler and runtime in kernel to replace paging for virtual address translation"

# DeepCOVID-XR is an deep learning algorithm for detecting COVID-19 on chest X-rays,trained and tested on the largest published clinical dataset in the COVID-19 era with performance similar to the consensus of experienced, cardiothoracic fellowship-trained thoracic radiologists.
tags: [Memory, Compiler, Runtime]
categories: [Memory System]
featured: true

# Custom links (optional).
#   Uncomment and edit lines below to show custom links.
# links:
# - name: Follow
#   url: https://twitter.com
#   icon_pack: fab
#   icon: twitter

url_pdf: https://dl.acm.org/doi/10.1145/3503222.3507771
url_code: https://github.com/SuchyB/CaratCakeArtifact
url_dataset:
url_poster:
url_project:
url_slides:
url_source:
url_video: https://www.youtube.com/watch?v=nYNFx3vAC2k

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
