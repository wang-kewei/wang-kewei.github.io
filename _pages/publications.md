---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

{% assign publications = site.publications | sort: "date" | reverse %}

<ol>
{% for publication in publications %}
  <li>
    <strong>{{ publication.title }}</strong><br>
    {{ publication.author | replace: "Kewei Wang", "<strong>Kewei Wang</strong>" }}. <em>{{ publication.venue }}</em>{% if publication.arxiv %}:{{ publication.arxiv }}{% endif %}{% if publication.volume %} {{ publication.volume }}{% endif %}{% if publication.issue %}({{ publication.issue }}){% endif %}{% if publication.article %}, {{ publication.article }}{% endif %}{% if publication.pages %}, {{ publication.pages }}{% endif %} ({{ publication.date | date: "%Y" }}). <a href="{{ publication.paperurl }}">[Link]</a>
  </li>
{% endfor %}
</ol>

See also my [Google Scholar profile](https://scholar.google.com/citations?user=qPCpNmYAAAAJ&hl=en).
