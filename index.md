---
layout: default
title: Home
nav_order: 1
description: C4 model
permalink: /
---

# 소프트웨어 아키텍처 시각화를 위한 C4 모델

C4 모델은 다음과 같습니다.

1. [계층적 추상화(hierarchical abstractions, 소프트웨어 시스템, 컨테이너, 컴포넌트 및 코드)](<(/abstractions)>)의 집합입니다.
2. [계층적 다이어그램(hierarchical diagrams, 시스템 컨텍스트, 컨테이너, 구성 요소 및 코드)](<(/diagrams)>)의 집합입니다.
3. [표기법에 독립적](/diagrams/notation)입니다.
4. [도구에 독립적](/tooling)입니다.

[![소프트웨어 아키텍처 시각화를 위한 C4 모델 개요]({{ site.baseurl }}/images/c4-overview.png)]({{ site.baseurl }}/images/c4-overview.png)

## 용도 및 이점

C4 모델은 배우기 쉽고 개발자 친화적인 소프트웨어 아키텍쳐 다이어그램에 대한 접근법입니다.
좋은 소프트웨어 아키텍처 다이어그램은 소프트웨어 개발/제품 팀 내외부의 커뮤니케이션,
신규 직원의 효율적인 온보딩, 아키텍처 검토/평가, 리스크 식별(예: [리스크 스토밍](https://riskstorming.com)),
위협 모델링 등에 도움이 됩니다.

<table style="text-align: center">
<tr>
<td>
<iframe src="https://www.youtube-nocookie.com/embed/x2-rSnhpw0g" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
<br />
<b>C4 모델을 사용한 소프트웨어 아키텍처 시각화</b>
<br />
2019년 7월 "Agile on the Beach 2019"에서 촬영
</td>
<td>
<a href="https://leanpub.com/visualising-software-architecture"><img src="{{ site.baseurl }}/images/book-small.png" width="150px" /></a>
<br />
<b>소프트웨어 아키텍처 시각화를 위한 C4 모델</b>
<br />Simon Brown
</td>
</tr>
</table>

<script>
    const links = {
        'abstractions': '/abstractions',
        'systemcontextdiagram': '/diagrams/system-context',
        'containerdiagram': '/diagrams/container',
        'componentdiagram': '/diagrams/component',
        'codediagram': '/diagrams/code',
        'systemlandscapediagram': '/diagrams/system-landscape',
        'dynamicdiagram': '/diagrams/dynamic',
        'deploymentdiagram': '/diagrams/deployment',
        'notation': '/diagrams/notation',
        'tooling': '/tooling',
        'faq': '/faq',
    };
    var hash = window.location.hash;

    if (hash && hash.length > 0) {
        hash = hash.substring(1).toLowerCase();
        const link = links[hash];

        if (link) {
            window.location.href = link;
        }
    }
</script>
