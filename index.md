---
layout: default
title: AllWeatherOS
---

<section class="hero">
  <p class="eyebrow">AllWeatherOS · Public Finance · Asset Allocation</p>
  <h1>경제의 모든 계절에 흔들리지 않는 금융 지식.</h1>
  <p>ISA·연금저축·IRP 같은 절세계좌를 중심으로 ETF, 채권, 금, 원자재, 리츠, 현금성 자산을 시민의 언어로 해석합니다.</p>
  <div class="cta-row">
    <a class="button" href="#latest">최신 포스팅 보기</a>
    <a class="button ghost" href="{{ '/about' | relative_url }}">운영 철학</a>
  </div>
</section>

<section class="principles">
  <div><strong>절세계좌 중심</strong><span>ISA·연금저축·IRP 관점으로 설명합니다.</span></div>
  <div><strong>잃지 않는 배분</strong><span>올웨더 철학과 위험관리를 우선합니다.</span></div>
  <div><strong>출처 기반</strong><span>중앙은행·정부·거래소·운용사 원문을 우선합니다.</span></div>
  <div><strong>투자 권유 아님</strong><span>판단 기준과 금융 문해력을 남깁니다.</span></div>
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
