---
layout: page
permalink: /projects/
title: projects
description: Open-source research and funded projects in remote sensing and digital cultural heritage.
nav: true
nav_order: 3
---

## Open-source research

<div class="projects">
  <div class="row row-cols-1 row-cols-md-3">
    {% assign sorted_projects = site.projects | sort: "importance" %}
    {% for project in sorted_projects %}
      {% include projects.liquid %}
    {% endfor %}
  </div>
</div>

## Current

- **Dynamic Monitoring and Risk Assessment of Large-Scale Linear Cultural Heritage** (2025–present)<br>
  National Key Research and Development Program of China, Project No. 2024YFB3908900.

- **Digital Fingerprint Authentication for Museum Collections** (2023–present)<br>
  National Key Research and Development Program of China, Project No. 2023YFF0906203.

## Completed

- **BeiDou and Space–Air–Ground Integrated Intelligent Surveying** (2023–2025)<br>
  National Key Research and Development Program of China, Project No. 2021YFB2600401.

- **Integrated Remote Sensing Archaeology and Ancient-Book Stitching** (2023–2024)<br>
  National Key Research and Development Program of China, Project No. 2020YFC1521903.

- **Multimodal Land-Use Interpretation** (2021–2023)<br>
  Open Fund project, Project No. KF-2021-06-088.

- **Building Instance Dataset Construction** (2020–2021)<br>
  National Earth Observation Data Center project, Project No. NODAOP2020015.

## Industry experience

- **Tencent CSIG**, Research Intern, June–August 2022.
