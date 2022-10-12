{% for item in include.list %}
- ({{ item.name}} )[{{ item.url }}] - {{ item.description }}
{% endfor %}
