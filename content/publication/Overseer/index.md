---
title: 'Overseer: Enforcing fine-grained memory access control across execution environments'

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here
# and it will be replaced with their full name and linked to their profile.
authors:
  - Darius Suciu
  - admin
  - Bin Sun
  - Radu Sion

# Author notes (optional)
#author_notes:
#  - 'Equal contribution'
#  - 'Equal contribution'

date: '2026-06-01T00:00:00Z'
doi: ''

# Schedule page publish date (NOT publication's date).
publishDate: '2026-06-01T00:00:00Z'

# Publication type.
# Accepts a single type but formatted as a YAML list (for Hugo requirements).
# Enter a publication type from the CSL standard.
publication_types: ['paper-conference']

# Publication name and optional abbreviated publication name.
publication: ACM Asia Conference on Computer and Communications Security (AsiaCCS)
#publication_short: In *ICW*

abstract: TrustZone enables Rich Execution Environments (REEs) and Trusted Execution Environments (TEEs) to share physical memory by building virtual address spaces without knowing each other’s mapping. While TEE hardware protection guarantees that the REE (“Normal World”) is restricted to accessing non-secure memory exclusively, the Secure OS and Trusted Applications (TAs) operating within the TEE (“Secure World”) can map physical memory belonging to REE OS and applications. As a result, vulnerabilities within TEE code, in conjunction with the inherent semantic gap between the REE and TEE can be leveraged by malicious actors to completely bypass REE security policies and leak or compromise REE-sensitive data or code. Our comprehensive analysis of TAs from commercial TrustZone devices and associated CVEs in the past decade has revealed numerous REE and TEE physical memory access vulnerabilities across multiple vendors. To mitigate the security impact of this critical semantic gap, we introduce Overseer, a secure monitor mechanism that prevents unauthorized physical memory mappings by TEEs, one of the important enablers of compromise. Overseer further enables the Secure OS and the TAs running inside the TEE to regulate the invocation of Secure Monitor Calls (SMCs) and System Calls. Overseer’s performance overhead is under 2% on average. A detailed CVE analysis shows that Overseer can mitigate the attack surface of over 53 TA vulnerabilities.


# Summary. An optional shortened abstract.
#summary: Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis posuere tellus ac convallis placerat. Proin tincidunt magna sed ex sollicitudin condimentum.

tags: []

# Display this page in the Featured widget?
featured: true

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: 'https://dl.acm.org/doi/pdf/10.1145/3779208.3807496'
url_code: 'https://github.com/sandeepkiranp/overseer'
url_dataset: ''
url_poster: ''
url_project: ''
url_slides: ''
url_source: ''
url_video: ''

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
