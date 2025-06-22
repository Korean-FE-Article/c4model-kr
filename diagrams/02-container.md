---
layout: default
title: 2. 컨테이너 다이어그램
parent: 다이어그램
nav_order: 2
permalink: /diagrams/container
---

# 컨테이너 다이어그램

시스템이 전반적인 IT 환경에서 어디에 위치하는지를 이해한 후에 컨테이너 다이어그램으로 시스템 경계 내부를 자세히 들여다보는 것은 아주 유용합니다. "컨테이너"는 서버 사이드 웹 애플리케이션, 싱글 페이지 애플리케이션(SPA), 데스크톱 애플리케이션, 모바일 앱, 데이터베이스 스키마, 파일 시스템 등과 같은 것을 의미합니다. 본질적으로 컨테이너는 코드를 실행하거나 데이터를 저장하는 독립적으로 실행/배포할 수 있는 단위(예: 별도의 프로세스 공간)입니다.

컨테이너 다이어그램은 소프트웨어 아키텍처의 상위 수준 형태와 책임이 어떻게 분산되어 있는지 보여줍니다. 또한 주요 기술 선택 사항과 컨테이너가 서로 어떻게 통신하는지 보여줍니다. 이는 소프트웨어 개발자와 지원/운영 직원 모두에게 유용한 단순하고 상위 수준의 기술 중심 다이어그램입니다.

## 예시

[![컨테이너 다이어그램](https://static.structurizr.com/workspace/36141/diagrams/Containers.png)](https://static.structurizr.com/workspace/36141/diagrams/Containers.png)

### 다이어그램 키

[![다이어그램 키](https://static.structurizr.com/workspace/36141/diagrams/Containers-key.png)](https://static.structurizr.com/workspace/36141/diagrams/Containers-key.png)

## 범위

단일 소프트웨어 시스템입니다.

## 주요 요소

범위 내 소프트웨어 시스템의 컨테이너입니다.

## 지원 요소

컨테이너에 직접 연결된 사람과 소프트웨어 시스템입니다.

## 대상 독자

소프트웨어 개발팀 내부 및 외부의 기술 인력으로, 소프트웨어 아키텍트, 개발자 및 운영/지원 직원을 포함합니다.

## 추천하시나요?

네, 컨테이너 다이어그램은 모든 소프트웨어 개발팀에게 권장됩니다.

## 참고 사항

이 다이어그램은 클러스터링, 로드 밸런서, 복제, 장애 조치 등에 대해 언급하지 않습니다. 이는 다양한 환경(예: 프로덕션, 스테이징, 개발 등)에서 달라질 가능성이 높기 때문입니다. 이 정보는 하나 이상의 [배포 다이어그램]({{ site.baseurl }}/diagrams/deployment)을 통해 더 잘 표현할 수 있습니다.

<script type="application/javascript" src="https://code.jquery.com/jquery-3.7.1.slim.min.js"></script>
<script type="application/javascript" src="/assets/c4model.js"></script>
