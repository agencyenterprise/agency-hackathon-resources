{% if include.category and site.data[include.parent][include.category.data] %}
### {% if include.category.icon %}{{ include.category.icon }}{% endif %} {{ include.category.label }} [📝]({{ site.repo_data_url }}/{{ include.parent }}/{{ include.category.data }}.yml)]
  {% for item in site.data[include.parent][include.category.data] %}
  - #### {% if site.data.content[item.data].icon %}{{ site.data.content[item.data].icon }}{% endif %} **{{ site.data.content[item.data].label }}**
    {% include linklist.md list=item.list %}
  {% endfor %}
{% endif %}
