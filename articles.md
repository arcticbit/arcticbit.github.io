---
layout: default
title: Arctic Bit
permalink: /articles
---

<div class="container" style="margin-top: 80px;min-height: 80vh">
    <div class="row">
        <div class="col s12">
            <ul>
            {% for post in site.posts %}
                <li>
                    <h3>
                        <a href="{{ post.url }}">{{ post.title }}</a>
                        <small style="display: block;font-size: .6em;text-transform:initial">Published by {{post.author}} on {{post.date | date: '%B %d, %Y' }}</small>
                    </h3>
                    <article style="text-align: justify; margin-bottom: 24px">
                        {{ post.excerpt}}
                    </article>
                    <a class="waves-effect waves-light btn-small" href="{{post.url}}">Read more</a>
                </li>
            {% endfor %}
            </ul>
        </div>
    </div>
</div>