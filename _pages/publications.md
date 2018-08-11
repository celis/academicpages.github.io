---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}



<a style="line-height: 1.5;" href="http://inspirehep.net/author/profile/A.Celis.1"><span style="color: #333333;"><span style="font-size: medium;">Available in INSPIRE.</span></span></a>
