{% if include.list and include.category and site.data[include.category][include.list] %}
### {% if include.icon %}{{ include.icon }}{% endif %} {{ include.label }} [[![external link](https://dafoster.net/assets/2018/external_link.png)]({{ site.repo_data_url }}/{{ include.category }}/{{ include.list }}.yml)]
  {% for category in site.data[include.category][include.list] %}
  - #### {% if category.icon %}{{ category.icon }}{% endif %} **{{ category.label }}**
    {% include linklist.md list=category.list %}
  {% endfor %}
{% endif %}
