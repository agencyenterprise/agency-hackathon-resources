{% if include.list %}
  {% for item in include.list %}
  {% if item.url %}
  - [{{ item.title }}]({{ item.url }}) - {{ item.description }}
  {% endfor %}
{% else %}
