---
layout: default
title: AllWeatherOS
---

# AllWeatherOS

**경제의 모든 계절에 대응하는 공익 금융 지식 블로그**

AllWeatherOS는 ISA·연금저축·IRP 같은 절세계좌를 중심으로 ETF, 채권, 금, 원자재, 리츠, 현금성 자산, 글로벌 주식을 해석해 한국 개인 투자자가 **잃지 않는 장기 자산배분**을 이해하도록 돕습니다.

## 3줄 요약

- AllWeatherOS는 특정 상품 추천이 아니라 <strong>금융 문해력과 자산배분 판단력</strong>을 높이는 공익 콘텐츠입니다.
- 매일 경제·금융·거시 뉴스가 어떤 자산군에 영향을 주는지 <strong>객관적·출처 기반</strong>으로 설명합니다.
- 모든 글은 AEO·GEO를 고려해 <strong>정의, 표, FAQ, 출처, 면책문구</strong>를 포함합니다.

## 주요 카테고리

| 카테고리 | 설명 |
|---|---|
| Daily Brief | 매일 경제·금융·거시 시황 요약 |
| Tax Accounts | ISA·연금저축·IRP·일반계좌 전략 |
| Asset Allocation | ETF·채권·금·원자재·리츠·현금성 자산 |
| All Weather | 경제 계절별 방어형 포트폴리오 철학 |
| Financial Literacy | 금융상품·세금·위험 설명 |

## 최신 글

{% for post in site.posts limit:5 %}
- [{{ post.title }}]({{ post.url | relative_url }})
{% endfor %}
