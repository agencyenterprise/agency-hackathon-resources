{{ include.flag }}
{{ include.list }}

{% for item in side.data.development.web.articles %}

{{ item.title }}
{{ item.url }}
( {{ item.title }} )[{{ item.url }}] - {{ item.description }}

{% endfor %}
