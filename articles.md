---
layout: default
title: Arctic Bit
permalink: /articles
---
<div class="splash-image" style="background: url('/assets/mountain-alt.png'); height: 400px;background-position: center center;filter: saturate(30%); background-size: cover;">
</div>
<div class="container" style="margin-top: 40px;min-height: 80vh">
    {% for post in site.posts %}
    <div class="row" style="margin-bottom: 40px;">
        <div class="col s12">
            <ul>
                <li>
                    <h3 style="margin: 0;padding:0;">
                        <a href="{{ post.url }}">{{ post.title }}</a>
                        <small style="display: block;font-size: .6em;text-transform:initial;margin-top:8px">Published by {{post.author}} on {{post.date | date: '%B %d, %Y' }}</small>
                    </h3>
                    <article style="text-align: justify; margin: 32px 0">
                        {{ post.excerpt}}
                    </article>
                    <a class="cta" href="{{post.url}}">Read more</a>
                </li>
            </ul>
        </div>
    </div>
            {% endfor %}
</div>