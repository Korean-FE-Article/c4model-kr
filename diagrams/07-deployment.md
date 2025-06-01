---
layout: default
title: Deployment diagram
parent: Diagrams
nav_order: 7
permalink: /diagrams/deployment
---

# 배포 다이어그램

배포 다이어그램을 통해 정적 모델의 소프트웨어 시스템 및/또는 컨테이너 인스턴스들이 특정 **배포 환경**(예: 프로덕션, 스테이징, 개발 등) 내의 인프라에 어떻게 배포되는지 시각화 할 수 있습니다. 이는 [UML 배포 다이어그램](https://en.wikipedia.org/wiki/Deployment_diagram)을 기반으로 합니다.

**배포 노드**는 소프트웨어 시스템/컨테이너의 인스턴스가 실행되는 위치를 나타냅니다. 물리적 인프라(예: 물리 서버나 기기), 가상화된 인프라(예: IaaS, PaaS, 가상 머신), 컨테이너화된 인프라(예: Docker 컨테이너), 실행 환경(예: 데이터베이스 서버, 자바 EE 웹/애플리케이션 서버, 마이크로소프트 IIS) 등일 수 있습니다. 배포 노드는 중첩될 수 있습니다.

DNS 서비스, 로드 밸런서, 방화벽 등과 같은 **인프라 노드**도 포함하고 싶을 수 있습니다. Amazon Web Services, Azure 등에서 제공하는 아이콘을 사용하여 배포 다이어그램을 보완해도 좋습니다. 단, 사용하는 모든 아이콘이 다이어그램 키/범례(legend)에 포함되어야 합니다.

## 예시 1

[![배포 다이어그램](https://static.structurizr.com/workspace/36141/diagrams/LiveDeployment.png)](https://static.structurizr.com/workspace/36141/diagrams/LiveDeployment.png)

### 다이어그램 키

[![다이어그램 키](https://static.structurizr.com/workspace/36141/diagrams/LiveDeployment-key.png)](https://static.structurizr.com/workspace/36141/diagrams/LiveDeployment-key.png)

## 예시 2

[![배포 다이어그램](https://static.structurizr.com/workspace/54915/diagrams/AmazonWebServicesDeployment.png)](https://static.structurizr.com/workspace/54915/diagrams/AmazonWebServicesDeployment.png)

### 다이어그램 키

[![다이어그램 키](https://static.structurizr.com/workspace/54915/diagrams/AmazonWebServicesDeployment-key.png)](https://static.structurizr.com/workspace/54915/diagrams/AmazonWebServicesDeployment-key.png)

## 범위

단일 배포 환경(예: 프로덕션, 스테이징, 개발 등) 내의 하나 이상의 소프트웨어 시스템입니다.

## 주요 요소 및 지원 요소

배포 노드, 소프트웨어 시스템 인스턴스, 컨테이너 인스턴스입니다.

## 지원 요소

소프트웨어 시스템 배포에 사용되는 인프라 노드입니다.

## 대상 독자

소프트웨어 개발팀 내외부의 기술 담당자들입니다. 소프트웨어 아키텍트, 개발자, 인프라 아키텍트, 운영/지원 스태프를 포함합니다.

## 추천하시나요?

네.

<script type="application/javascript" src="https://code.jquery.com/jquery-3.7.1.slim.min.js"></script>
<script type="application/javascript" src="/assets/c4model.js"></script>
