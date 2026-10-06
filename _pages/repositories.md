---
layout: page
permalink: /repositories/
title: repositories
description: The repositories behind the <a href='/projects'>projects</a>.
nav: true
nav_order: 5
---

## GitHub Repositories

<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% for repo in site.data.repositories.github_repos %}
    {% include repository/repo.liquid repository=repo %}
  {% endfor %}
</div>