{% if include.list and include.category %}
{{ include.list }}
{{ include.category }}
{% for category in site.data[include.category][include.list] %}
- {{ category.label }}
  {% include linklist.md list=category.list %}
{% endfor %}
{% endif %}
