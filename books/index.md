# Book Recommendations

{% for post in site.categories.books %}
  <a href="{{ post.url }}">{{ post.title }}</a>
{% endfor %}
