---
layout: page
permalink: /repositories/
title: repositories
description: Here is my Github that hosts all my work.
nav: true
nav_order: 4
---

{% if site.data.repositories.github_users %}

## [Github](www.github.com/debkal)

---

---

## GitHub Repositories

<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% for repo in site.data.repositories.github_repos %}
    {% include repository/repo.liquid repository=repo %}
  {% endfor %}
</div>
{% endif %}
