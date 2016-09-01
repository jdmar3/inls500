---
layout: default
---
<h1>{{ page.title }}</h1>

{% capture datestamp %}{{page.date | date: "%F"}}{% endcapture %}
{% capture today %}{{site.time | date: "%F"}}{% endcapture %}
<p class="subtitle">{{ page.date | date: "%A, %-d %B %Y" }}{% if datestamp == today  %}&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span class="smaller date contrast">TODAY</span>{% endif %}</p>

{{ content }}

<p>
  <br/>
  <ul class="tags">
    {% for tag in page.tags %}<li><a href="/topics#{{ tag }}" class="tag">{{ tag | replace: " ", "-" }}</a></li>{% endfor %}
  </ul> 
</p>