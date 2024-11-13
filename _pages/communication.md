---
layout: page
permalink: /meetings/
title: Meetings
---

## Calendar 
<iframe src="https://calendar.google.com/calendar/embed?height=400&wkst=2&ctz=Europe%2FZurich&showPrint=0&showTitle=0&showDate=0&showTabs=0&mode=AGENDA&src=NzYyNGQ0YWRhNDE2YjI3YzdmYmE2YTcxMmI4OWNiZjY3OTdiZGJkNzc4NzgyNjVlYmNhNTEwOThhYThhNzk0NUBncm91cC5jYWxlbmRhci5nb29nbGUuY29t&color=%23039BE5" style="border-width:0" width="100%" height="400" frameborder="0" scrolling="no"></iframe>

## Agendas and minutes

<div id="archives">
  <section id="archive">
     <h3>Most Recent Posts</h3>
      {%for post in site.posts %}
      {% unless post.next %}
      <ul class="this">
          {% else %}
          {% capture month %}{{ post.date | date: '%B %Y' }}{% endcapture %}
          {% capture nmonth %}{{ post.next.date | date: '%B %Y' }}{% endcapture %}
          {% capture year %}{{ post.date | date: '%Y' }}{% endcapture %}
          {% capture nyear %}{{ post.next.date | date: '%Y' }}{% endcapture %}
          {% if year != nyear %}
      </ul>
      <h2 style="text-align:left;">{{ post.date | date: '%Y' }}</h2>
      <ul class="past">
          {% endif %}
          {% if month != nmonth %}
          <h3 style="text-align:left;">{{ post.date | date: '%B %Y' }}</h3>
          {% endif %}
          {% endunless %}
          <p><b><a href="{{ site.baseurl }}{{ post.url }}">{% if post.title and post.title != "" %}{{post.title}}{% else %}{{post.excerpt |strip_html}}{%endif%}</a></b> - {% if post.date and post.date != "" %}{{ post.date | date: "%e %B %Y" }}{%endif%}</p>
          {% endfor %}
      </ul>
    <h3>Oldest Posts</h3>
  </section>
</div>


