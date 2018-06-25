# Assessment breakdown

{% marginnote 'tab1' '*Table 1*: List of required course tasks' %}

| **Assignment** | **Corresponding learning objectives** | **%** | **Due date** |  
| :------- | :------------- | ----: | -----------: |{% for post in site.categories.assignments reversed %}{% if post.title %}
| [{{ post.short_description }}]({{ post.url | prepend: site.baseurl }}) | {{ post.objectives }} | {{ post.percentage }} | {{ post.start_date | date: "%b %-d at %H:%M" }} |{% endif %}{% endfor %}
| Class discussion / participation | 3,4,5 | 20 | Ongoing |