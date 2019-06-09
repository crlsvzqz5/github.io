---
layout: default
title: home
---

## Welcome!

Select a topic on the left to begin exploring. 

<div style="position:relative; top:100px;">
{% for item in site.data.home_topics %}
<a href="javascript:downTree('{{ item.link }}');">
<figure class="topic_fig">
<img class="topic_img" src="{{ item.image }}"/>
<figcaption>{{ item.caption }}</figcaption>
</figure>
<!-- <button onclick="downTree('/fpga_topics.html')">click</button> -->
</a>
{% endfor %}
</div>
