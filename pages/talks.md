---
title: Talks
permalink: /talks/
---

# Talks
<div class="flex flex-wrap -mx-2">
    {% for talk in site.talks %}
        <div class="w-full sm:w-1/2 lg:w-1/3 mb-4 px-2">
            <a href="{{ talk.url }}">
            <div class="card overflow-hidden rounded-lg">
                <div class="w-full h-48" 
                    style="background-size: cover; 
                    background-position: center; 
                    background-image: url('/images/talks/{{ talk.thumbnail }}');
                    ">
                </div>
                <div class="p-8">
                    <h4 class="text-xs">{{ talk.conference }}</h4>
                    {{ talk.title }}
                </div>
           </div>
           </a>
        </div>
    {% endfor %}
</div>
