---
layout: home
---

# Agency Hackathon Resources

This is a collection of useful resources to supercharge your next agency increasing hackathon project. [Feel free to contribute](https://github.com/ianribeiroae/agency-hackathon-resources) with your own material, just try to keep it as high quality as possible so people can go straight to the good stuff.

Not sure if your agency-increasing project is agency-ready? Check out the [Ultimate Hackathon Guide](https://docs.google.com/document/d/1j6U0tsVgsT5KKHBAZaurcgm4L6zHj_OhNyw7NPvMj1U/edit?usp=sharing).

{% include content_summary.html %}

{% for category in site.data.categories %}
## {{ category.label }}
  {% for item in category.list %}
{% include category.md parent=category.data category=item %}
  {% endfor %}
{% endfor %}
