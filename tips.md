---
layout: default
title: Tips
breadcrumb:
- Home
- Tips
---

# Tips!

<ul>
	{% for page in site.pages %}
		{% if page.layout == "tip" %}
			<li><a href="{{ page.url | relative_url }}">{{ page.title }}</a></li>
		{% endif %}
	{% endfor %}
</ul>
