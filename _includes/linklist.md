{% if include.list %}
  {% for item in include.list %}
    {% if item.url and item.title %}
    - [{{ item.title }}]({{ item.url }}){% if item.description %} - {{ item.description }}{% endif %}
    {% endif %}
  {% endfor %}
{% endif %}
