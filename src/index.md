---
# Feel free to add content and custom Front Matter to this file.

layout: default
---
<div style="display: flex; gap: 50px; padding: 3rem 0;">
  <div>
    <h1 style="margin: 0;">👋🏻 My name is</h1>
    <h1 style="margin: 0; color: #177ead">Justin Marsh</h1>
    <div style="padding: 1rem 1rem 1rem 0;">
      Full Stack Ruby on Rails Software Engineer 🤓, Tango Dancer 💃🏻,
      and Cooking Enthusiast 👨🏻‍🍳. This is my personal website where I
      document my journey as a full stack developer and publish tutorials for myself
      and others on things I’ve learned along the way.
      <br/><br/>
      Current Project: [TangotubeTV](https://tangotube.tv)
    </div>
  </div>
  <div style="margin: auto;">
    <img src="<%= relative_url '/images/main-avatar.jpg' %>"
        alt="Logo"
        class="avatar avatar--main" />
  </div>
</div>


<div style="display: flex; gap: 1rem; padding: 6rem 1rem;">
  <div style="flex: 1;">
    <h3 style="margin: 0;">What I Do</h3>
    <h2 style="margin: 0;">Full Stack Developer</h2>
    Here are things about me that may interest you. There listed like it's some sort of dating profile. Maybe I will be able to woo you over.
  </div>
  <div style="flex: 1;">
    <div>
      <h2>Ruby on Rails</h2>
      <p>3 years building with the world's most productive web framework</p>
    </div>
    <div>
      <h2>Sass</h2>
      <p>I'm a bit of a traditionalist in this sense, I prefer clean markup, but I'm not opposed to other frameworks.</p>
    </div>
    <div>
      <h2>Hotwire</h2>
      <p>The fastest way to build interactive websites</p>
    </div>
    <div>
      <h2>DevOps</h2>
      <p>I usually use Digital Ocean with a Ubuntu droplet. My web servers are usually NGINX or Apache</p>
    </div>
  </div>
  <div style="flex: 1;">
    <div>
      <h2>Databases</h2>
        <p>
          Full-Text-Search <br>
          (Elastic Search, Meilisearch, Postgres Native)
        </p>
    </div>
    <div>
      <h2>Javascript</h2>
        <p>
          Vanilla Javascript
        </p>
        <p>
          TypeScript
        </p>
        <p>
          StimulusJS
        </p>
    </div>
    <div>
      <h2>UI/UX</h2>
      <p> I'm not afraid to get my hands dirty with tools like Figma or Adobe XD</p>
    </div>
        <div>
      <h2>Testing</h2>
      <p> Rspec</p>
    </div>
    <div>

    </div>
  </div>
</div>

## Recent Posts
<div class="post">
  <% collections.posts.resources.each do |post| %>
  <a href="<%= post.relative_url %>">
    <h2><%= post.data.title %></h2>
    <p><%= post.data.description %></p>
    <%= post.data.date.strftime('%d %b %Y') %>
    </a>
  <% end %>
</div>

