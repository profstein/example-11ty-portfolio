---
title: Graphic Design
layout: base.njk
tags: navItem
---
<main class="design cards">
    <h2 class="cards_header">Graphic Design Projects</h2>
    {%- for page in collections.design %}
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