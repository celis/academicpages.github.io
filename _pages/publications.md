---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---



<a style="line-height: 1.5;" href="http://inspirehep.net/author/profile/A.Celis.1"><span style="color: #474791;"><span style="font-size: medium;">See complete list in INSPIRE.</span></span></a>

<p>Last publication:</p>




{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}

<br/><img src='/images/500x300.png'>

