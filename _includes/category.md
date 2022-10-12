{% if include.category %}
{% for category in include.category %}
- category.label
  {% for category_list in category.list %}
    {% include linklist.md list=category_list %}
  {% endfor %}
{% endfor %}
{% endif %}
