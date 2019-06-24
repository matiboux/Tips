---
layout: default
title: Home
breadcrumb:
- Home
---

# {{ site.title }}

<div class="alert alert-info">
	<h4 class="alert-heading">This is a BETA project!</h4>
	<p class="mb-0">Help by contributing to <a href="{{ site.github.repository_url }}">the open-source repository</a>! <i class="fas fa-heart fa-fw text-danger"></i></p>
</div>

Hi.

## Tips!

<ul>
	{% for page in site.pages %}
		{% if page.layout == "tip" %}
			<li><a href="{{ page.url | relative_url }}">{{ page.title }}</a></li>
		{% endif %}
	{% endfor %}
</ul>
