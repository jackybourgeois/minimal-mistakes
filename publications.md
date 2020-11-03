---
title: Publications
layout: collection
permalink: /publications/
author_profile: true
---

{% assign sorted = site['publications'] | sort: 'year' | reverse %}
{% for publication in sorted %}
[{{ publication.type }}] {{ publication.authors }}. {{ publication.title }}. {{ publication.venue }}. {{ publication.year }}
{% endfor %}