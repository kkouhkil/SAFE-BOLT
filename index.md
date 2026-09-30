---
layout: default
title: Home
---
<section class="section split home-intro">
  <div>
    <p class="eyebrow">{{ site.data.site.mission }}</p>
    <h1>SAFE-<span>BOLT</span></h1>
    <h2>{{ site.data.site.project_full_name }}</h2>
  </div>
  <div class="body-copy hero-copy-right">
    <p>{{ site.data.home.hero_description }}</p>
    <div class="actions">
      <a class="button primary" href="{{ '/project/' | relative_url }}">Explore the project</a>
      <a class="button secondary" href="{{ '/demo/' | relative_url }}">Watch progress</a>
    </div>
    <div class="hero-meta"><span>{{ site.data.site.institution }}</span><span>{{ site.data.site.phase }}</span><span>{{ site.data.site.focus_area }}</span></div>
  </div>
</section>

<section class="section split">
  <div><p class="eyebrow">THE PROJECT</p><h2>From scientific plans to reliable physical execution.</h2></div>
  <div class="body-copy"><p>{{ site.data.home.project_summary }}</p><p><a class="text-link" href="{{ '/project/' | relative_url }}">Read the project overview →</a></p></div>
</section>

<section class="section dark">
  <div class="section-inner">
    <p class="eyebrow">RESEARCH PIPELINE</p><h2>From demonstration to deployment.</h2>
    <div class="pipeline">{% for item in site.data.home.pipeline %}<article><span>0{{ forloop.index }}</span><h3>{{ item.title }}</h3><p>{{ item.text }}</p></article>{% endfor %}</div>
  </div>
</section>

<section class="section">
  <p class="eyebrow">APPLICATIONS</p><h2>Representative laboratory workflows.</h2>
  <div class="feature-grid">
    <article class="feature-card"><span class="card-kicker">01</span><h3>Materials Synthesis & Assembly</h3><p>Liquid and powder dispensing combined with contact-rich mechanical assembly, including alignment, insertion and fastening.</p></article>
    <article class="feature-card"><span class="card-kicker">02</span><h3>Microscope-Centered Optofluidics</h3><p>Microliter pipetting, glass and film handling, and interaction with laboratory instrument controls.</p></article>
  </div>
  <p><a class="text-link" href="{{ '/applications/' | relative_url }}">Explore applications →</a></p>
</section>

<section class="section">
  <p class="eyebrow">LATEST PROGRESS</p><h2>A living record of SAFE-BOLT development.</h2>
  <div class="news-grid">{% for post in site.posts limit:3 %}<article class="feature-card"><span class="post-date">{{ post.date | date: "%d %b %Y" }}</span><h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3><p>{{ post.excerpt | strip_html | truncate: 170 }}</p></article>{% endfor %}</div>
  <p><a class="text-link" href="{{ '/news/' | relative_url }}">View all updates →</a></p>
</section>
