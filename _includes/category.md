{{ include }}

{% if include.list %}
{% for category in data[include.category][include.list] %}
- category.label
  {% include linklist.md list=category.list %}
{% endfor %}
{% endif %}
