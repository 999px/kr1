---
layout: default
---
<div style="background-color: #F00">113</div>
<div id="gallery">
{% for img in site.static_files %}
  {% if img.path contains 'images/' %}
    <a href="{{ img.path | relative_url }}"><img src="{{ img.path | relative_url }}" width="150"></a>
  {% endif %}
{% endfor %}
</div>