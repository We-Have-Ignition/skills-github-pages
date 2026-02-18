---
layout: default
---
Here I’ll share thoughts and code related to:

- Market microstructure
- HFT strategies

<h2 class="post-list-heading">Posts</h2>

<ul class="post-list">
{% for post in site.posts %}
  <li>
    <span class="post-meta">
      {{ post.date | date: "%b %-d, %Y" }}
    </span>
    <h3>
      <a class="post-link" href="{{ post.url | relative_url }}">
        {{ post.title }}
      </a>
    </h3>

    {%- comment -%} Optional excerpt under the title {%- endcomment -%}
    {%- if post.excerpt -%}
      <p>{{ post.excerpt | strip_html | truncate: 180 }}</p>
    {%- endif -%}
  </li>
{% endfor %}
</ul>
