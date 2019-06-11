---
layout: default
title: home
---

## Welcome!

Select a topic on the left to begin exploring. 

<div style="position:relative; top:100px;">
{% for item in site.data.home_topics %}
<a href="#" onclick="changeTreeNode('{{ item.link }}', this); return false;" id="link_atnode0" class="topiclinkHOME">
<figure class="topic_fig">
<img class="topic_img" src="{{ item.image }}"/>
<figcaption>{{ item.caption }}</figcaption>
</figure>
</a>
{% endfor %}
</div>
