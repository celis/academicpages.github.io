---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}


<a style="line-height: 1.5;" href="https://celis.github.io/files/cv.pdf"><span style="color: #333333;"><span style="font-size: medium;">Full CV available in PDF format.</span></span></a>



<p>Short version:</p>


{% include base_path %}
{% capture written_label %}'None'{% endcapture %}

<h1 class="western" align="center"><b>Alejandro Celis</b></h1>
<p style="line-height: 1.5;" align="center"><span style="font-size: medium;"><b>Curriculum Vitae</b> </span></p>
<p style="line-height: 1.5;" align="center"><span style="font-size: medium;">  <a href="https://celis.github.io">https://celis.github.io</a> | <a href="https://twitter.com/alej_celis">@alej_celis</a> | <a href="https://scholar.google.de/citations?hl=en&user=l0kb_3kAAAAJ">Google Scholar</a></span></p>

<h2 class="western">Education:</h2>
<ul style="line-height: 1.5; margin: 10px 0;">
 	<li><span style="font-size: medium;"><b>Ph.D., </b></span><strong><span style="font-size: medium;"><b>Information Management and Systems with a designated emphasis in New Media</b></span></strong><span style="font-size: medium;"><b>, University of California at Berkeley</b></span>

<h2 class="western">Research Interests and Skills:</h2>
<ul style="line-height: 1.5; margin: 10px 0;">
 	<li><span style="font-size: medium;"><b>Topical:</b> collaboration, socialization, literacy, and governance in distributed, decentralized communities, specifically new/social media platforms and scientific research networks</span></li>
 	<li><span style="font-size: medium;"><b>Disciplinary:</b> social informatics, computer-supported cooperative work (CSCW), science and technology studies (STS), data science studies, critical algorithm studies, media and communication studies, organizational sociology, critical human-computer interaction (HCI)</span></li>
 	<li><span style="font-size: medium;"><b>Theoretical:</b> socio-technical systems, communities of practice, ethnomethodology, symbolic interactionism, distributed cognition, actor-network theory, phenomenology</span></li>
 	<li><span style="font-size: medium;"><b>Methodological:</b></span>


<h2>Employment</h2>
<ul style="line-height: 1.5; margin: 10px 0;">
  <li><span style="font-size: medium;"><b>Postdoctoral scholar and staff ethnographer</b>, UC-Berkeley Institute for Data Science (Jan 2016 to present)</span></li>
  <li><span style="font-size: medium;"><b>Research Intern</b>, Wikimedia Foundation (May to August 2011)</span></li>
</ul>
<h2>Summary of Scholarly Impact</h2>
<ul style="line-height: 1.5; margin: 10px 0;">

  <li><span style="font-size: medium;"><b>Publications:</b> 22 publications with 961 total citations, h-index of 15 (Google Scholar)</li>
  <li><span style="font-size: medium;"><b>Presentations:</b> Over 50 talks, including 7 invited talks and 2 conference keynotes</li>
  <li><span style="font-size: medium;"><b>Industry:</b> Scholarship has directly led to new initiatives and redesigned products at Wikimedia</li>
</ul>
<h2>Publications</h2>
  <ul>{% for post in site.articles %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>

<h2>Talks</h2>
  <ul>{% for post in site.talks %}
    {% unless post.talk_type == "Conference proceedings talk" %}
      {% include archive-single-talk-cv.html %}
    {% endunless %}
  {% endfor %}</ul>

<h2>Teaching</h2>
  <ul>{% for post in site.teaching %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>




