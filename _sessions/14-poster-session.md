---
day: 2
day_title: "August 12, 2026 (Day 2)"
order: 7
time: "16:40 - 17:30"
name: poster-session
title: "NVMSA Poster Session"
---
**Session Chair:** Tianyu Wang  

{% assign poster_papers = site.papers | where: "poster", true | sort: "id" %}
{% for paper in poster_papers %}
- **[{{ paper.title }}](#){: data-target="{{ paper.id }}" .modal-trigger }**  
  {{ paper.author }}
{% endfor %}
