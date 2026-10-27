---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

<a href="{{ base_path }}/files/Yang-Wu-CV.pdf">Download CV (PDF)</a>

Education
======
* Ph.D. in Computer Science, Worcester Polytechnic Institute, Worcester, MA, May 2026
  * Dissertation: *Advancing the Proactive Capacity of LLMs in Cost-Sensitive Domains*
  * Advisor: Xiaozhong Liu
* M.P.S. in Analytics, Northeastern University, Boston, MA, Apr 2021
* B.S. in Material Engineering, Wuhan University, Wuhan, China, Jun 2018

Appointments
======
* AI Research Scientist II, Axon, Boston, MA, Apr 2026 – present
* Research Assistant / Teaching Assistant, Worcester Polytechnic Institute, Worcester, MA, Aug 2021 – Mar 2026
* 2025 Intern, Research Scientist / Engineer, Adobe, San Jose, CA, May 2025 – Aug 2025
* Software Engineer Intern (AML-Enterprise), ByteDance, San Jose, CA, May 2024 – Aug 2024
* Bioinformatics Intern, EMD Serono Research Center, Billerica, MA, Jan 2020 – Jun 2020

Research
======
* Trustworthy NLP and large language models, combining data-efficient training, human-centered feedback, and domain-adaptive reasoning, applied to legal reasoning, biomedical discovery, personalized education, and public safety.
* Lead projects on data-efficient LLM training, proactive LLM assistants, multimodal LLM systems, and generative AI applications.
* 16 peer-reviewed articles at ACL, EMNLP, NAACL, CIKM, WWW, and AAAI workshops, with additional papers under review and in preparation.

Publications
======
{% for category in site.publication_category %}
{% assign title_shown = false %}
{% for post in site.publications reversed %}
{% if post.category != category[0] %}
{% continue %}
{% endif %}
{% unless title_shown %}
<h2>{{ category[1].title }}</h2>
<ul>
{% assign title_shown = true %}
{% endunless %}
{% include archive-single-cv.html %}
{% endfor %}
{% if title_shown %}
</ul>
{% endif %}
{% endfor %}

Oral presentations
======
<ul>
{% for post in site.talks reversed %}
{% include archive-single-talk-cv.html %}
{% endfor %}
</ul>

Teaching
======
<ul>
{% for post in site.teaching reversed %}
{% include archive-single-cv.html %}
{% endfor %}
</ul>

Selected projects
======
* **Team+1: Proactive LLM Assistants for Scientific Discovery** (Project lead, 2025 – present). A proactive assistant that anticipates when to intervene and precomputes reasoning offline for low-latency biomedical collaboration.
* **Data-Efficient LLM Training** (Project lead, 2024 – present). A reward-oriented, active-learning framework that keeps the training examples most useful for instruction tuning.
* **Human-Centered and Multimodal LLM Assistants** (Project lead, 2023 – present). Assistants for legal reasoning, personalized tutoring, and camera-controlled video generation.

Awards
======
* AAAI 2026 AI-Law Bridge Best Paper Award, The 40th AAAI Conference on Artificial Intelligence Bridge between Artificial Intelligence and Law, 2026
* Rank No. 2, Food for Thought Challenge Competition, United States Department of Agriculture, 2023

Service
======
* Reviewer, AAAI 2027 (4 papers)
* Reviewer, NeurIPS 2026 (4 papers)
* Reviewer, AAAI 2026 (4 papers)
* Reviewer, EMNLP 2026 (4 papers)
* Reviewer, ACL 2026 (8 papers)
* Reviewer, CoNLL 2026 (2 papers)
* Reviewer, ACL 2025 (16 papers)
* Reviewer, EMNLP 2025 (4 papers)
* Reviewer, EACL 2025 (2 papers)
* Reviewer, CIKM 2024 (2 papers)
