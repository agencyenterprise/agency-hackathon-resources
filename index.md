---
layout: home
---

# Agency Hackathon Resources

This is a collection of useful resources to supercharge your next agency increasing hackathon project. [Feel free to contribute](https://github.com/ianribeiroae/agency-hackathon-resources) with your own material, just try to keep it as high quality as possible so people can go straight to the good stuff.

{% include content_summary.html %}

---

{% for category in site.data.categories %}
## {{ category.label }}
  {% for item in category.list %}
{% include category.md category=category.data item=item %}
  {% endfor %}
{% endfor %}
