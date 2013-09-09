---
layout: page
---
{% include JB/setup %}



<ul class="posts">
  {% for post in site.posts %}
  <!--  <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>  -->

    <li>
            <h2>
              <a href="{{ post.url }}">{{ post.title }}</a>
            </h2>
            <div style="color: #999;">
              <span class="title-desc">{{ post.description }}</span>
            </div>
          
        </li>

  {% endfor %}
</ul>



