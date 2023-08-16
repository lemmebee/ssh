---
layout: about
title: about
permalink: /
# subtitle: <a href='#'>Affiliations</a>. Address. Contacts. Moto. Etc.

profile:
  align: right
  image: e____.png
  image_circular: false # crops the image to make it circular
  # address: >
  #   <p>Lyon, France</p>

news: false  # includes a list of news items
latest_posts: false  # includes a list of the newest posts
selected_papers: false # includes a list of papers marked as "selected={true}"
social: true  # includes social icons at the bottom of the page
---

Hey! I'm a Software Engineer who is passionate about writing code and thinking about how things work. Nerdy at the moment about the realm of DevOps! But beyond the lines of code and terminal screens, I hold my breath and dive as deep as I can in the sea - Please don't judge me by only my glasses.

<h1 class="post-title">Latest Projects</h1>
{% if site.data.repositories.github_repos %}
<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% for repo in site.data.repositories.github_repos %}
    {% include repository/repo.html repository=repo %}
  {% endfor %}
</div>
{% endif %}
