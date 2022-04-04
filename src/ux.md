---
title: UX
layout: base.njk
tags: navItem
---
<main class="uiux cards">
    <h2 class="cards_header">UI/UX Projects</h2>
    {%- for page in collections.ux %}
    <div class="pjcard">
      <div class="card_img">
          <a href="{{page.url}}"><img src="/images/{{page.data.postImg}}" alt="{{page.data.postImgAlt}}"></a></div>
      <div class="card_text">
        <h3><a href="{{page.url}}">{{page.data.title}}</a></h3>
        <p>{{page.data.description}}<p>
      </div>
    </div> 
    </div>
    {%- endfor %}
</main>