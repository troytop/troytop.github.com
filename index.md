---
layout: page
title: Welcome
posts: 5
---

<img src="/images/tt-2007-sm.jpg" alt="Troy Topnik" style="float:right; padding:10px; width:100px" />
I am a software product manager, technical writer, and fiddler with technology and software. I worked for many years for ActiveState and now work for HPE.

Apologies for the lack of... well, everything. The site is grossly incomplete, but under actual construction soon. 

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
