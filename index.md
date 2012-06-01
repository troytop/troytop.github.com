---
layout: page
title: Welcome
posts: 5
---

<img src="/images/tt-2007-sm.jpg" alt="Troy Topnik" style="float:right; padding:10px; width:100px" />
I am a writer and fiddler with technology and software. I work as a technical copywriter, sales engineer, and undefinable entity for ActiveState.

Apologies for the lack of... well, everything. I've copied this Jekyll style from <a target="_new" href="https://github.com/dueyfinster/dueyfinster.github.com/">Neil Grogan's repo</a> and hopefully purged all references to his stuff. The site is grossly incomplete, but under actual construction now. 

In the meantime, there are lots of posts by me on the [ActiveState
Blog](http://www.activestate.com/blog/authors/troyt). 

<aside id="recent-posts">
<h2>Recent Blog Posts:</h2>

<!-- Start of Display Recent Posts -->
<table class="posts">
<!-- Get 7 most recent entries by date (asc) -->
 {% for post in site.posts limit:7 offset:0 %}
 <tr>
               <th>{{ post.date | date_to_string }}</th>
      <td><a href='{{ post.url }}'>{{ post.title }}</a></td>         
 </tr>
      {% endfor %} 
             </table>
</aside>
<!-- End of Display Recent Posts -->
