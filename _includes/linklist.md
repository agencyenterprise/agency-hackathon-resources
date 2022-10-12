{{ include.flag }}

{% for item in include.list %}

{{ include.list }}
{{ item.title }}
{{ item.url }}
( {{ item.title }} )[{{ item.url }}] - {{ item.description }}

{% endfor %}
