---
# Feel free to add content and custom Front Matter to this file.

layout: default
---
<div>
  <img src="<%= relative_url '/images/main-avatar.jpg' %>"
      alt="Logo"
      class="avatar avatar--main" />
</div>
<h1 style="margin: 0;">Justin Marsh</h1>

testing cname 2

Full Stack Ruby on Rails Software Engineer 🤓, Tango Dancer 💃🏻,
and Cooking Enthusiast 👨🏻‍🍳. This is my personal website where I
document my journey as a full stack developer and publish tutorials for myself
 and others on things I’ve learned along the way.

Current Project: [TangotubeTV](https://tangotube.tv)

<h2>Recent Posts</h2>
<div class="post">
  <% collections.posts.resources.each do |post| %>
  <a href="<%= post.relative_url %>">
    <h2><%= post.data.title %></h2>
    <p><%= post.data.description %></p>
    <%= post.data.date.strftime('%d %b %Y') %>
    </a>
  <% end %>
</div>

----
