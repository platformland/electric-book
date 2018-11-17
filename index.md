---
title: Home
style: home
---

{% include metadata %}

# {{ project-name }}

{{ project-description }}

{% for book in site.data.meta.works %}
*[{{ book.title }}]({{ book.directory }}/text/{{ book.products.web.start-page }}.html)*
{% endfor %}


