---
web_templates:
  -
    name: "AwesomeReactBoilerplate"
    description: "My awesome boilerplate for React. Woo!"
    link: "https://github.com/ianribeiroae/agency-hackathon-resources"
  -
---

{% for template in page.web_templates %}
- ({{ template.name}} )[{{ template.link }}] - {{ template.description }}
{% endfor %}
