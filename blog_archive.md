---
permalink: /blog
layout: page
title: Blog
---

{% comment %}
{% for tag in site.tags %}
  <div style="    border: none;
    border-radius: 0.8em;
    display: inline-block;
    background-color: lightgray;
    padding: 0.3em;
    margin: 0.5em;">{{ tag[0] }}</div>
  <ul>
    {% for post in tag[1] %}
        <li>
            <a href="{{ post.url }}">{{ post.title }}</a>            
        </li>
    {% endfor %}
  </ul>
{% endfor %}
{% endcomment %}


  
  <ul>
    {% for post in site.posts %}
        <li style="display:block;margin-bottom:1.5em;">            
            <span style="font-size: small;color: gray;">
                    published on {{ post.date | date: "%b %d, %y" }}
            </span>
            <br/>
            <a href="{{ post.url }}">{{ post.title }}</a>
            <br/>
            {% for tag in post.tags %}
                <span style="border-radius: 0.8em;padding: 0.3em;;background-color: lightgray;;margin:.3em;font-size:small;padding-top:.1em;margin-left:0em;">
                    {{ tag }}
                </span>                
            {% endfor %}            
        </li>
    {% endfor %}
  </ul>
