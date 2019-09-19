---
layout: default
title: Arctic Bit
permalink: /articles
---


<div class="container" style="min-height: 80vh">
    <div class="row" style="margin: 0 -10px;">
    {% for post in site.posts %}
        <div class="col s12 m6" style="padding: 0 20px">
            <div style="background-image: url('{{ post.splash }}'); background-position: center center; background-size: cover; height: 300px;margin-bottom: 30px">
            </div>        
                    <h4 style="margin: 0;padding:0;">
                        <a href="{{ post.url }}">{{ post.title }}</a>
                        <small style="display: block;font-size: .6em;text-transform:initial;margin-top:8px">Published by {{post.author}} on {{post.date | date: '%B %d, %Y' }}</small>
                    </h4>
                    <article style="text-align: justify; margin: 32px 0;height: 240px">
                        {{ post.excerpt}}
                    </article>
                    <div class="right-align">
                        <a class="cta" href="{{post.url}}">Read more</a>
                    </div>
        </div>
            {% endfor %}
    </div>
</div>