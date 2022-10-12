{% if include.list and include.category and site.data[include.category][include.list] %}
  {% for category in site.data[include.category][include.list] %}
  - {% if category.icon %}{{ category.icon }}{% endif %} **{{ category.label }}**
    {% include linklist.md list=category.list %}
  {% endfor %}
{% endif %}
