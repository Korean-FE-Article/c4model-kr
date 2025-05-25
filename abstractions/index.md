---
layout: default
title: Abstractions
nav_order: 3
has_children: true
permalink: /abstractions
has_toc: false
---

# 추상화

"코드의 지도"를 만들기 위해서는 먼저, 소프트웨어 시스템의 정적 구조를 설명할 수 있는 공통된 추상화 세트가 필요합니다. C4 모델에서는,

> [소프트웨어 시스템](./01-software-system.md)은
> 하나 이상의 [컨테이너](./02-container.md)(애플리케이션과 데이터 저장소)로 구성되고,
> 각 컨테이너는 하나 이상의 [컴포넌트](./03-component.md)를 포함하며, 이 컴포넌트들은
> 하나 이상의 [코드](./04-component.md) 요소(클래스, 인터페이스, 객체, 함수 등)로 구현됩니다.
> 그리고 사람들(액터, 역할, 페르소나, 특정 개인 등)은 우리가 만든 소프트웨어 시스템을 사용합니다.

![The abstractions behind the C4 model](/images/abstractions.png)

C4 모델은 소프트웨어 아키텍처를 다이어그램으로 표현하는 "추상화 우선" 접근법입니다.
이 모델은 소프트웨어 아키텍트와 개발자들이 소프트웨어에 대해 생각하고 구축하는 방식을 반영하는 추상화를 기반으로 합니다. 적은 수의 추상화와 다이어그램 유형 덕분에 C4 모델은 배우기 쉽고 사용하기 간단합니다.
