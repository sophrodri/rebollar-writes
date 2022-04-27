---
layout: post 
title: Sophie's Journal 
description: A log of Sophie's poems and short stories 
order: 3
___

{{site.title}}
{{site.description}}
{% include menu.html %}

    
       <!-- Create a loop -->
    {% for block in site.data.journal.story %}
    <div class="cards">
<div class="card">
    <div class="pic">
        <img src="{{block.image}}" alt="{{block.image-alt}}">
    </div>
        <div class="content">
            <h3 class="title">{{block.title}}</h3>
           <h4>{{block.subtitle}}</h4>
           <p>{{block.story-content}}</p>
           <p><a href="{{block.tag-link}}">{{block.tag}}</a></p>
        </div>
    </div>
</div>
{% endfor %}


{% include credits.html%}
