---
tag_page_dir: tag
tag_page_layout: tag_page
tag_permalink_style: pretty
tag : blog
---

<div class='o-wrapper'>

  <div class='o-grid'>
    <div class='o-grid__col'>
      <h4>{{ page.tag }}</h4>
    </div>
  </div>

  <div class='o-grid'>
    {% for post in page.posts %}
      {% include post-card.liquid %}
    {% endfor %}
  </div>

  <div class='o-grid'>
    {% include pagination.html %}
  </div>
</div>