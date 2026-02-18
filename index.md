---
---
Here I’ll share thoughts and code related to:

- Market microstructure
- HFT strategies

{% raw %}
{% for post in site.posts %}
### [{{ post.title }}]({{ post.url | relative_url }})

{{ post.excerpt | strip_html | truncate: 180 }}
{% endfor %}
{% endraw %}
