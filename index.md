---
layout: default
---

text_112<br>
<div id="gallery">
{% for img in site.static_files %}
  {% if img.path contains './images/' %}
    <a href="{{ img.path }}"><img src="{{ img.path }}" width="150"></a>
  {% endif %}
{% endfor %}
</div>