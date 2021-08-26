# Hackers Choice

A curated collection of products and services recommended by the fine folks at [Hacker News](https://news.ycombinator.com)

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>
