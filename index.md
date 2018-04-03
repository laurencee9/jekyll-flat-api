---
layout: default
---

<!-- Load the squares -->
<div class="thumbnails-content row">
{% for node in site.documentation %}
{% if node.thumbnail == true %}
<div class="col-sm-5 thumbnail">{{ node.content }} </div>
{% endif %}
{% endfor %}
</div>

<!-- Load the content -->
{% for node in site.documentation %}
  {% if node.front == true %}
  {{ node.content }}
  {% for subpage in site.documentation %}
  {% if subpage.front == false and subpage.permalink contains node.permalink and subpage.thumbnail != true %}
  {{ subpage.content }}
  {% endif %}
  {% endfor %}
  {% endif %}
{% endfor %}

