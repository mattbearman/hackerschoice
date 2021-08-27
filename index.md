# Hackers Choice

A curated collection of products and services recommended by the fine folks at [Hacker News](https://news.ycombinator.com)

{% for category in site.categories %}
  <a href="/{{ category[0] }}">{{ category[0] }}</a>
{% endfor %}