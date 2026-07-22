---
layout: default
---

<section class="hero">
  <p class="eyebrow">올웨더경제 · AllWeatherOS · Economy · Asset Allocation</p>
  <h1>예측보다 대비를 말하는 경제·자산배분 아카이브.</h1>
  <p>성장과 침체, 인플레이션과 디플레이션처럼 서로 다른 경제 환경을 읽고, 주식·채권·현금성 자산·원자재·부동산·환율·절세계좌의 역할과 위험을 원칙 중심으로 해석합니다.</p>
  <div class="cta-row">
    <a class="button" href="#latest">최신 포스팅 보기</a>
    <a class="button ghost" href="{{ '/about' | relative_url }}">운영 철학</a>
  </div>
  <figure class="hero-visual">
    <img src="{{ '/assets/images/hero/allweatheros-hero.png' | relative_url }}" alt="경제 환경의 변화와 자산배분 원칙을 상징하는 편집 이미지" loading="eager">
  </figure>
</section>

<section class="principles" aria-label="올웨더경제의 편집 원칙">
  <div><strong>관측</strong><span>금리·물가·환율·정책으로 경제 환경의 변화를 읽습니다.</span></div>
  <div><strong>구성</strong><span>자산별 역할과 위험을 이해하는 배분 원칙을 살핍니다.</span></div>
  <div><strong>지속</strong><span>ISA·연금·세금·현금흐름을 장기 금융생활과 연결합니다.</span></div>
  <div><strong>출처 기반</strong><span>중앙은행·정부·거래소·국제기구 원문을 우선합니다.</span></div>
</section>

<section id="latest">
  <h2>최신 포스팅</h2>
  <div class="post-list">
    {% for post in site.posts limit:12 %}
      <article class="post-card">
        {% if post.image %}
        <a class="post-thumb-link" href="{{ post.url | relative_url }}" aria-label="{{ post.title }}">
          <img src="{{ post.image | relative_url }}" alt="{{ post.image_alt | default: post.title }}" loading="lazy">
        </a>
        {% endif %}
        <p class="date">{{ post.date | date: "%Y.%m.%d" }}</p>
        <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
        <p>{{ post.description | default: post.excerpt | strip_html | truncate: 140 }}</p>
        <a class="read-more" href="{{ post.url | relative_url }}">읽기 →</a>
      </article>
    {% endfor %}
  </div>
</section>
