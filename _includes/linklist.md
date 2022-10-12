{% for item in include.list %}
- ( {{ item.title }} )[{{ item.url }}] - {{ item.description }}
{% endfor %}
