# Hackers Choice

A curated collection of products and services recommended by the fine folks at [Hacker News](https://news.ycombinator.com)

## Categories

{% for member in site.data.categories %}
  <a href="/{{ member.slug }}">
    {{ member.name }}
  </a>
{% endfor %}
