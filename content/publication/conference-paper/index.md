---
title: 'INVISILINE: Invisible Plausibly-Deniable Storage'

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here
# and it will be replaced with their full name and linked to their profile.
authors:
  - admin
  - Bogdan Carbunar
  - Anrin Chakraborti
  - Radu Sion

# Author notes (optional)
#author_notes:
#  - 'Equal contribution'
#  - 'Equal contribution'

date: '2023-07-01T00:00:00Z'
doi: ''

# Schedule page publish date (NOT publication's date).
publishDate: '2023-01-01T00:00:00Z'

# Publication type.
# Accepts a single type but formatted as a YAML list (for Hugo requirements).
# Enter a publication type from the CSL standard.
publication_types: ['paper-conference']

# Publication name and optional abbreviated publication name.
publication: IEEE Symposium on Security and Privacy (SP)
#publication_short: In *ICW*

abstract: Plausibly-deniable (PD) storage systems allow users to securely hide data and plausibly deny its presence when challenged by adversaries who coerce them to provide encryption keys and passwords. However, PD systems need specialized software that renders them detectable by suspicious adversaries questioning the very use of a PD system. To address this fundamental problem, we introduce and formally define the notion of plausible invisibility, preventing adversaries from determining whether a PD system was used in the first place. We develop INVISILINE, a plausibly invisible system resilient against multi-snapshot adversaries that can access the device multiple times. To remain invisible, INVISILINE uses a data layout and encoding that is compatible with the Linux dmcrypt disk encryption subsystem, and stores hidden data in the initialization vectors used by dm-crypt to encrypt public data. INVISILINE ensures that any disk changes that result from changes to the hidden data between adversary snapshots, can be plausibly explained using changes to public data resulting from regular use of dm-crypt. In the presence of adversaries, INVISILINE enables users to access all and only the public data using only dm-crypt. INVISILINE can securely and invisibly hide 19GB on a 1TB disk with no impact on public data I/O, and an average of 4.5 MB/s throughput for writing hidden data.

# Summary. An optional shortened abstract.
#summary: Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis posuere tellus ac convallis placerat. Proin tincidunt magna sed ex sollicitudin condimentum.

tags: []

# Display this page in the Featured widget?
featured: true

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: ''
url_code: 'https://www.computer.org/csdl/proceedings-article/sp/2024/313000a018/1RjE9Voxxkc'
url_dataset: 'https://github.com/HugoBlox/hugo-blox-builder'
url_poster: ''
url_project: ''
url_slides: ''
url_source: 'https://github.com/HugoBlox/hugo-blox-builder'
url_video: 'https://youtube.com'

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
#image:
#  caption: 'Image credit: [**Unsplash**](https://unsplash.com/photos/pLCdAaMFLTE)'
#  focal_point: ''
#  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
#projects:
#  - example

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
#slides: example
---

{{% callout note %}}
Click the _Cite_ button above to demo the feature to enable visitors to import publication metadata into their reference management software.
{{% /callout %}}

{{% callout note %}}
Create your slides in Markdown - click the _Slides_ button to check out the example.
{{% /callout %}}

Add the publication's **full text** or **supplementary notes** here. You can use rich formatting such as including [code, math, and images](https://docs.hugoblox.com/content/writing-markdown-latex/).
