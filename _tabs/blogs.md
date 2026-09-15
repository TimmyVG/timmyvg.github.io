---
layout: page
icon: fa-solid fa-newspaper
order: 1
title: Blogs
---

<div class="row row-cols-1 g-3">
{% assign posts = site.posts | sort: "date" | reverse %}
{% for post in posts %}
  <div class="col">
    <div class="card h-100 position-relative">
      <div class="card-body">
        <h5 class="card-title">
          <a href="{{ post.url | relative_url }}" class="stretched-link text-decoration-none">
            {{ post.title }}
          </a>
        </h5>
        <p class="card-text text-muted">
          {{ post.date | date: "%d %b %Y" }}
        </p>
      </div>
    </div>
  </div>
{% endfor %}
</div>
