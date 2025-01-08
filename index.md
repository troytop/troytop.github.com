---
layout: page
title: Welcome
posts: 5
---

<img src="/images/tt-2007-sm.jpg" alt="Troy Topnik" style="float:right; padding:10px; width:100px" />

I am a product manager with 25 years of experience in the software industry working with open source and open standard technologies. I look for opportunities to define software based on customer needs and work closely with development teams to help them deliver great products.

I have been a technical support engineer, technical writer, instructor, product manager, and enthusiastic user of a wide variety of open source software, focused on Cloud Foundry projects related to Kubernetes, such as KubeCF, Quarks, Eirini, Stratos, and Minibroker (CNCF). I work at [SUSE](https://suse.com) managing the [Rancher](https://www.rancher.com/products/rancher-platform) [partner ecosystem](https://www.suse.com/pcsc/home#search?platforms=1027).

<aside id="recent-posts">
<h2>Crufty Blog Posts:</h2>

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
