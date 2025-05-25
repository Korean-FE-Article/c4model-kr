---
layout: default
title: Introduction
nav_order: 2
permalink: /introduction
---

# 개요

건설 업계 전문가에게 건물 구조를 시각적으로 표현해 달라고 하면, 그들은 보통 배치도, 평면도, 입면도, 단면도, 그리고 상세 도면을 보여줄 것입니다.
반대로 소프트웨어 개발자에게 다이어그램을 사용하여 소프트웨어 시스템의 소프트웨어 아키텍처를 표현해 달라고 요청하면 박스와 선이 뒤섞인 혼란스러운 그림, 일관성 없는 표기법(색상 코딩, 모양, 선 스타일 등), 모호한 이름, 레이블 없는 관계, 일반적 용어, 잘못된 기술 선택, 혼합 추상화 등을 보게 될 가능성이 높습니다.

| [![소프트웨어 아키텍처 스케치](/images/sketch-1.jpg)](/images/sketch-1.jpg) | [![소프트웨어 아키텍처 스케치](/images/sketch-2.jpg)](/images/sketch-2.jpg) |
| --------------------------------------------------------------------------- | --------------------------------------------------------------------------- |
| [![소프트웨어 아키텍처 스케치](/images/sketch-3.jpg)](/images/sketch-3.jpg) | [![소프트웨어 아키텍처 스케치](/images/sketch-4.jpg)](/images/sketch-4.jpg) |

업계에는 통합 모델링 언어(UML), ArchiMate, SysML이 존재하지만, 이러한 언어가 소프트웨어 아키텍처를 효과적으로 전달하는 방법을 제공하는지를 묻는 것은 종종 무의미합니다. 많은 팀이 훨씬 더 간단한 "박스와 선" 다이어그램을 선호하기 때문입니다. 이러한 모델링 언어를 포기한 것 자체는 괜찮을 수 있지만, 속도를 중요시 여기는 개발 문화 속에서, 많은 소프트웨어 개발 팀이 시각적으로 소통하는 능력을 잃어버린 것은 아닐까 생각합니다.

## 코드의 지도

C4 모델은 소프트웨어 개발 팀이 소프트웨어 아키텍처를 더 잘 설명하고 전달할 수 있도록 돕기 위해 개발되었습니다. 이는 Google 지도 등을 사용할 때 관심 있는 영역을 확대 및 축소하는 것과 같은 방식으로 다양한 세부 수준의 '코드 지도'를 만드는 방법으로, 사전 설계 단계에서의 논의 뿐만 아니라 기존 코드베이스를 나중에 문서화 할 때에도 활용될 수 있습니다.

| [![](/images/map-4.jpg)](/images/map-4.jpg)                                                                                                                  | [![](/images/map-3.jpg)](/images/map-3.jpg)                                                                                                     | [![](/images/map-2.jpg)](/images/map-2.jpg)                                                                      | [![](/images/map-1.jpg)](/images/map-1.jpg)                                                                                                                       |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [![](https://static.structurizr.com/workspace/36141/diagrams/SystemContext.png)](/diagrams/system-context)                                                   | [![](https://static.structurizr.com/workspace/36141/diagrams/Containers.png)](/diagrams/container)                                              | [![](https://static.structurizr.com/workspace/36141/diagrams/Components.png)](/diagrams/component)               | [![](https://static.structurizr.com/workspace/36141/diagrams/MainframeBankingSystemFacade.png)](/diagrams/code)                                                   |
| 레벨 1: [시스템 컨텍스트 다이어그램](/diagrams/system-context)은 스코프 내의 소프트웨어 시스템이 주변 환경에 어떻게 들어맞는지 보여주는 시작점을 제공합니다. | 레벨 2: [컨테이너 다이어그램](/diagrams/container)은 소프트웨어 시스템의 스코프를 확대하여 그 내부의 애플리케이션과 데이터 저장소를 보여줍니다. | 레벨 3: [컴포넌트 다이어그램](<(/diagrams/component)>)은 개별 컨테이너를 확대해 그 내부의 컴포넌트를 보여줍니다. | 레벨 4: [코드 다이어그램](/diagrams/code)(예: UML 클래스)을 사용하여 개별 컴포넌트를 확대하여 해당 컴포넌트가 코드 수준에서 어떻게 구현되는지 보여줄 수 있습니다. |

## 다이어그램 성숙도 향상

C4 모델의 목표는 소프트웨어 아키텍처 다이어그램에 대한 성숙도를 높이는 것입니다.

[![](/images/software-architecture-diagramming-maturity-model.png)](/images/software-architecture-diagramming-maturity-model.png)

<script type="application/javascript" src="https://code.jquery.com/jquery-3.7.1.slim.min.js"></script>
<script type="application/javascript" src="/assets/c4model.js"></script>
