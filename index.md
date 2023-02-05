---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---
# Hackers Choice

A curated collection of products and services recommended by the fine folks at [Hacker News](https://news.ycombinator.com)

{% for collection in site.collections %}
  {% unless collection.label == "posts" %}
 - {{ collection.label }}{% for thing in collection.docs %}
   - [{{ thing.title }}]({{ thing.url }})
  {% endfor %}
  {% endunless %}
{% endfor %}