{% for thing in include.things %}
## [{{ thing.name }}]({{ thing.url }})

{% if thing.subtitle %}_{{ thing.subtitle }}_{% endif %}

{% if thing.image %}![{{ thing.name }} cover]({{ thing.image }}){% endif %}

{{ thing.description }}

### Recommended in these threads:

{% for thread in thing.hn_threads %}
- [{{ thread.title }}](https://news.ycombinator.com/item?id={{ thread.id }}){% endfor %}
{% if thing.hn_search %}- [And many more]({{ thing.hn_search }}){% endif %}

---

{% endfor %}