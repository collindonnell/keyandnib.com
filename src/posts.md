---
layout: page
title: Blog
permalink: /blog/
---

<% if site.collections.posts.docs.empty? %>
  <h2>No posts yet.</h2>
<% else %>
  <section id="posts-list">
    <% site.collections.posts.each do |post| %>
      <p>
        <%= post.data[:date].strftime('%m/%d/%y') %> - <a href="<%= post.url %>"><%= post.data[:title] %></a>
      </p>
    <% end %>
  </section>
<% end %>
