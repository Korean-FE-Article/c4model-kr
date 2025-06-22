---
layout: default
title: Tooling
nav_order: 6
permalink: /tooling
---

# 도구 선택(Tooling)

설계 세션에서는 협업과 빠른 반복 작업을 위해 화이트보드나 플립차트 용지가 더 나을 수 있습니다. 장기적으로 사용될 문서의 경우, C4 모델을 기반으로 소프트웨어 아키텍처 다이어그램을 만드는 데 도움이 되는 여러 도구가 있습니다. 도구를 살펴볼 때 다음과 같은 몇 가지 질문을 스스로에게 던져보세요.

- 다이어그램을 작성한 사람은 누구이며, 얼마나 기술적인가요?
- 다이어그램의 대상 독자는 누구이며, 그들은 어떻게 다이어그램/문서에 접근할까요?
- [다이어그래밍 vs 모델링?]({{ site.baseurl }}/images//tooling#diagramming-vs-modelling)
- "드래그 앤 드롭 UI" vs "코드로 된 다이어그램"?
- 데이터를 소스 코드와 가까운 git에 저장 vs 도구/클라우드 서비스에 저장?
- 풀 리퀘스트에 사용할 소스를 쉽게 구분할 수 있나요?
- 폐쇄형 데이터 형식인가요? 개방형 데이터 형식인가요?
- 인터랙티브 다이어그램인가요? 정적 다이어그램인가요?
- 무료인가요? 유료인가요?
- 클로즈드 소스인가요? 오픈 소스인가요?
- 클라우드를 사용하나요? 셀프호스팅하나요?
- 단기(Short-lived) 문서화인가요? 장기(Long-lived) 문서화인가요?
- 팀 전용 다이어그래밍인가요? 전사적(enterprise-wide) 모델링인가요?
  그

## 다이어그래밍 vs 모델링

다이어그래밍과 모델링에 대해 간략히 설명하겠습니다. 툴 사용과 관련하여 가장 중요한 결정이기 때문입니다. C4 모델은 다이어그래밍 툴이든 모델링 툴이든 상관없이 사용할 _수_ 있지만, 다이어그래밍에서 모델링으로 전환할 때 흥미로운 기회들이 있습니다.

### 다이어그래밍

업계에서는 모델링(예: Sparx EA, Archi, IcePanel, Structurizr 등)보다 다이어그래밍(예: Visio, draw.io, Lucidchart, PlantUML, Mermaid 등)을 선호하는 경향이 있습니다. 주된 이유는 진입 장벽이 상대적으로 낮고 훨씬 간단한 작업으로 여겨지기 때문입니다. 하지만 소프트웨어 아키텍처 다이어그램에 다이어그래밍 도구를 사용하는 데에는 몇 가지 큰 문제가 있습니다.

1. 다이어그래밍 도구의 도메인 언어는 "상자와 선"입니다. 이는 다음을 의미합니다.

- 그것들은 당신의 다이어그램에 대한 어떠한 도움이나 검증도 제공할 수 없습니다.
- 다이어그램을 쿼리할 수 없습니다(예: "구성 요소 X의 모든 종속성을 보여주세요").

2. 다이어그램 요소를 재사용하려면 복사-붙여넣기를 사용해야 합니다. 즉, 상자의 이름을 바꾸면 해당 상자가 나타나는 모든 다이어그램에서 상자의 이름을 바꿔야 합니다.
3. 많은 다이어그래밍 도구가 차이를 비교하기 힘든 데이터 구조를 갖고 있기 때문에 풀 리퀘스트와 함께 사용하기가 까다로운 경우가 많습니다.

### 모델링

모델링 도구를 사용하면 소프트웨어 아키텍처의 비시각적 모델(모든 요소와 요소 간의 관계에 대한 단일 정의)을 구축한 다음 그 모델에 대해 다양한 뷰(다이어그램이 되는)를 만들 수 있습니다. 모델링 도구는 사용자가 하려는 작업의 의미를 이해하고 추가적인 지원을 제공하며 요소/관계의 이름을 쉽게 변경할 수 있으므로 문제를 해결할 수 있습니다.

소프트웨어 아키텍처 모델은 본질적으로 노드와 에지로 구성된 [유향 그래프](https://en.wikipedia.org/wiki/Directed_graph) 이며, 다이어그램은 그래프의 하위 집합을 보여줍니다. 모델(구조화된 데이터)과 뷰(다이어그램으로 표현되는)를 분리하면 여러 가지 흥미로운 가능성이 생긴다는 것을 금방 알 수 있습니다.

- 대규모의 복잡한 아키텍처 모델을 이해하는 데 도움이 되는 대체 시각화 만들기 - 자세한 내용은 [C4 모델은 확장 가능한가요?]({{ site.baseurl }}/faq#does-the-c4-model-scale)를 참고하세요.
- 모델 쿼리.
- 모델을 다른 도구로 내보내기.
- 그 외

모델은 단지 데이터일 뿐입니다! 그리고 소프트웨어 개발자인 우리는 그 데이터를 시각화하고 조작할 수 있는 도구를 무궁무진하게 보유하고 있습니다.

## 옵션

다음은 C4 모델의 특정 부분에 대한 지원을 제공하는 도구 모음입니다.

<script type="application/javascript" src="https://code.jquery.com/jquery-3.7.1.slim.min.js"></script>

<style>
.toolingOptionFilter {
    margin: 10px 20px 20px 10px;
    display: inline-block;
}
.toolingOption {
    font-size: 16px;
    display: inline-block;
    margin: 10px;
    border: solid 1px #1168BD;
    padding: 5px 10px 5px 10px;
    border-radius: 5px;
}
.toolingOption:hover {
    background: #1168BD;
    color: #ffffff;
}
.toolingOption:hover a {
    color: #ffffff;
}
.toolingOption a {
    text-decoration: none;
}
.toolingOption a:hover {
    background: #1168BD;
    color: #ffffff;
    text-decoration: none;
}
.centered {
    text-align: center;
}
.faded {
    opacity: 0.2;
}
.small {
    font-size: 13px;
}
.smaller {
    font-size: 11px;
}
</style>

<table>
<tr>
<td style="vertical-align: top">
    <h4>지원되는 다이어그램 유형</h4>
    <div class="toolingOptionFilter">
        <label><input id="toolingStaticDiagramsFilter" type="checkbox" checked="checked" disabled="disabled"> 정적 다이어그램</label>
        <div class="smaller">(예: 시스템 컨텍스트, 컨테이너 및 컴포넌트 다이어그램)</div>
    </div>

    <div class="toolingOptionFilter">
        <label><input id="toolingDynamicDiagramsFilter" type="checkbox"> 동적 다이어그램</label>
        <div class="smaller">(예: 협업 또는 시퀀스 다이어그램)</div>
    </div>

    <div class="toolingOptionFilter">
        <label><input id="toolingDeploymentDiagramsFilter" type="checkbox"> 배포 다이어그램</label>
        <div class="smaller">(예: 배포 및 인프라 문제를 보여주는 다이어그램)</div>
    </div>

</td>
<td style="vertical-align: top">
    <h4>다이어그래밍 vs 모델링</h4>
    <div class="toolingOptionFilter">
        <label><input id="toolingDiagrammingFilter" name="diagramVsModel" type="radio"> 다이어그래밍 도구</label>
        <div class="smaller">(상자와 화살표는 복사 및 붙여넣기를 통해 재사용되며, 보조 기능이나 유효성 검사 규칙 등이 없습니다.)</div>
    </div>

    <div class="toolingOptionFilter">
        <label><input id="toolingModelBasedFilter" name="diagramVsModel" type="radio" checked="checked"> 여러 다이어그램에서 요소를 재사용</label>
        <div class="smaller">(즉, 여러 다이어그램을 요소의 이름을 바꿀 때 자동으로 동기화하기 위한 모델링 도구)</div>
        <div style="margin-top: 10px">
        <span class="smaller" style="font-weight: normal; background: #02b621; color: #ffffff; padding: 5px; margin-top: 10px;">추천</span>
        </div>
    </div>

</td>
<td style="vertical-align: top">
    <h4>작성(Authoring)</h4>
    <div class="toolingOptionFilter">
        <label><input id="toolingWithUIFilter" name="authoring" type="radio"> 그래픽 유저 인터페이스</label>
        <div class="smaller">(드래그 앤 드롭 모델링 UI)</div>
    </div>

    <div class="toolingOptionFilter">
        <label><input id="toolingAsCodeFilter" name="authoring" type="radio" checked="checked"> 코드로서의 다이어그램과 모델</label>
        <div class="smaller">(쉬운 버전 관리 및 빌드 파이프라인/기타 도구와의 통합을 위해)</div>
    </div>

</td>
<td style="vertical-align: top">
    <h4>기타</h4>
    <div class="toolingOptionFilter">
        <label><input id="toolingOpenSourceFilter" type="checkbox"> 오픈소스</label>
        <div class="smaller">(무료, 포크/커스터마이즈 등)</div>
    </div>

    <div class="toolingOptionFilter">
        <label><input id="toolingRenderingToolIndependentFilter" type="checkbox"> 렌더링 도구에 독립적</label>
        <div class="smaller">(<a href="/diagrams/notation#alternative-visualisations">다이어그램, 그래프 등</a>과 같은 다양한 도구 또는 시각화 방식으로 다이어그램을 렌더링하기 위해)</div>
    </div>

</td>
</tr>
</table>

<div class="centered">
    <div class="toolingOption toolingOpenSource toolingModelBased toolingWithUI toolingStaticDiagrams toolingDynamicDiagrams toolingDeploymentDiagrams">
        <a href="https://www.archimatetool.com/blog/2020/04/18/c4-model-architecture-viewpoint-and-archi-4-7/" target="_blank">Archi</a>
    </div>
    <div class="toolingOption toolingOpenSource toolingDiagramming toolingAsCode toolingStaticDiagrams">
        <a href="https://github.com/lonely-lockley/archinsight" target="_blank">Archinsight</a>
    </div>
    <div class="toolingOption toolingModelBased toolingWithUI toolingStaticDiagrams toolingDeploymentDiagrams">
        <a href="https://www.archipeg.com/learn/c4-model-v1-metamodel" target="_blank">Archipeg</a>
    </div>
    <div class="toolingOption toolingModelBased toolingWithUI toolingStaticDiagrams toolingDynamicDiagrams toolingDeploymentDiagrams">
        <a href="https://github.com/ChangeVision/astah-c4model-plugin" target="_blank">Astah</a>
    </div>
    <div class="toolingOption toolingOpenSource toolingDiagramming toolingAsCode toolingStaticDiagrams toolingDynamicDiagrams toolingDeploymentDiagrams">
        <a href="https://github.com/plantuml-stdlib/C4-PlantUML" target="_blank">C4-PlantUML</a>
    </div>
    <div class="toolingOption toolingOpenSource toolingDiagramming toolingAsCode toolingStaticDiagrams toolingDynamicDiagrams toolingDeploymentDiagrams">
        <a href="https://adrianvlupu.github.io/C4-Builder" target="_blank">c4builder</a>
    </div>
    <div class="toolingOption toolingOpenSource toolingModelBased toolingAsCode toolingStaticDiagrams">
        <a href="https://github.com/SlavaVedernikov/C4InterFlow" target="_blank">C4InterFlow</a>
    </div>
    <div class="toolingOption toolingOpenSource toolingWithUI toolingDiagramming toolingStaticDiagrams">
        <a href="https://github.com/archivisio/c4_modelizer" target="_blank">C4 Modelizer</a>
    </div>
    <div class="toolingOption toolingOpenSource toolingDiagramming toolingAsCode toolingStaticDiagrams toolingDeploymentDiagrams">
        <a href="https://github.com/8T4/c4sharp" target="_blank">C4Sharp</a>
    </div>
    <div class="toolingOption toolingOpenSource toolingDiagramming toolingAsCode toolingStaticDiagrams">
        <a href="https://owulveryck.github.io/cue4puml4c4/" target="_blank">CUE4Puml4C4</a>
    </div>
    <div class="toolingOption toolingOpenSource toolingDiagramming toolingAsCode toolingStaticDiagrams">
        <a href="https://diagrams.mingrammer.com/docs/nodes/c4" target="_blank">Diagrams</a>
    </div>
    <div class="toolingOption toolingOpenSource toolingDiagramming toolingWithUI toolingStaticDiagrams toolingDynamicDiagrams toolingDeploymentDiagrams">
        <a href="https://www.diagrams.net/blog/c4-modelling" target="_blank">diagrams.net</a>
    </div>
    <div class="toolingOption toolingWithUI toolingDiagramming toolingStaticDiagrams toolingDynamicDiagrams toolingDeploymentDiagrams">
        <a href="https://libraries.excalidraw.com/#dmitry-burnyshev-c4-architecture" target="_blank">Excalidraw</a>
    </div>
    <div class="toolingOption toolingWithUI toolingDiagramming toolingStaticDiagrams toolingDynamicDiagrams toolingDeploymentDiagrams">
        <a href="https://www.figma.com/templates/c4-model-examples/" target="_blank">Figma</a>
    </div>
    <div class="toolingOption toolingWithUI toolingOpenSource toolingModelBased toolingStaticDiagrams toolingDynamicDiagrams toolingDeploymentDiagrams">
        <a href="https://gaphor.org" target="_blank">Gaphor</a>
    </div>
    <div class="toolingOption toolingWithUI toolingDiagramming toolingStaticDiagrams toolingDynamicDiagrams toolingDeploymentDiagrams">
        <a href="https://www.gliffy.com/blog/c4-model" target="_blank">Gliffy</a>
    </div>
    <div class="toolingOption toolingWithUI toolingModelBased toolingStaticDiagrams toolingDynamicDiagrams">
        <a href="https://icepanel.io/c4-model" target="_blank">IcePanel</a>
    </div>
    <div class="toolingOption toolingOpenSource toolingDiagramming toolingAsCode toolingStaticDiagrams toolingDynamicDiagrams toolingDeploymentDiagrams">
        <a href="https://keadex.dev/en/projects/keadex-mina" target="_blank">Keadex Mina</a>
    </div>
    <div class="toolingOption toolingWithUI toolingDiagramming toolingStaticDiagrams toolingDynamicDiagrams toolingDeploymentDiagrams">
        <a href="https://www.lucidchart.com/pages/templates/c4-model-example" target="_blank">Lucidchart</a>
    </div>
    <div class="toolingOption toolingWithUI toolingDiagramming toolingStaticDiagrams toolingDynamicDiagrams toolingDeploymentDiagrams">
        <a href="https://github.com/pihalve/c4model-visio-stencil" target="_blank">Microsoft Visio</a>
    </div>
    <div class="toolingOption toolingOpenSource toolingDiagramming toolingAsCode toolingStaticDiagrams toolingDynamicDiagrams toolingDeploymentDiagrams">
        <a href="https://mermaid.js.org/syntax/c4.html" target="_blank">Mermaid</a>
    </div>
    <div class="toolingOption toolingWithUI toolingDiagramming toolingStaticDiagrams toolingDynamicDiagrams toolingDynamicDiagrams toolingDeploymentDiagrams">
        <a href="https://miro.com/miroverse/c4-architecture/" target="_blank">Miro</a>
    </div>
    <div class="toolingOption toolingOpenSource toolingModelBased toolingAsCode toolingStaticDiagrams toolingDynamicDiagrams toolingDeploymentDiagrams">
        <a href="https://github.com/goadesign/model" target="_blank">Model</a>
    </div>
    <div class="toolingOption toolingOpenSource toolingWithUI toolingDiagramming toolingStaticDiagrams toolingDynamicDiagrams toolingDeploymentDiagrams">
        <a href="https://architecture.models.nasdanika.org/references/eSubpackages/c4/index.html" target="_blank">Nasdanika Architecture</a>
    </div>
    <div class="toolingOption toolingWithUI toolingDiagramming toolingStaticDiagrams toolingDynamicDiagrams toolingDeploymentDiagrams">
        <a href="https://stenciltown.omnigroup.com/stencils/c4/" target="_blank">OmniGraffle</a>
    </div>
    <div class="toolingOption toolingOpenSource toolingModelBased toolingAsCode toolingStaticDiagrams toolingDynamicDiagrams toolingDeploymentDiagrams">
        <a href="https://github.com/soulspace-org/overarch" target="_blank">Overarch</a>
    </div>
    <div class="toolingOption toolingOpenSource toolingModelBased toolingAsCode toolingStaticDiagrams toolingDynamicDiagrams toolingDeploymentDiagrams">
        <a href="https://github.com/DrMarkusVoss/pumla/blob/main/test/examples/C4example/pumlaC4Example.md" target="_blank">pumla</a>
    </div>
    <div class="toolingOption toolingOpenSource toolingModelBased toolingAsCode toolingStaticDiagrams">
        <a href="https://github.com/nielsvanspauwen/pystructurizr" target="_blank">PyStructurizr</a>
    </div>
    <div class="toolingOption toolingWithUI toolingModelBased toolingStaticDiagrams toolingDynamicDiagrams toolingDeploymentDiagrams">
        <a href="http://www.sparxsystems.eu/c4/" target="_blank">Sparx Enterprise Architect</a>
    </div>
    <div class="toolingOption toolingOpenSource toolingModelBased toolingAsCode toolingStaticDiagrams">
        <a href="https://rdbmodel.github.io" target="_blank">RDB modeling</a>
    </div>
    <div class="toolingOption toolingModelBased toolingWithUI toolingStaticDiagrams">
        <a href="https://revision.app/c4-model" target="_blank">Revision</a>
    </div>
    <div class="toolingOption toolingOpenSource toolingModelBased toolingAsCode toolingRenderingToolIndependent toolingStaticDiagrams toolingDynamicDiagrams toolingDeploymentDiagrams">
        <a href="https://structurizr.com" target="_blank">Structurizr</a>
    </div>
    <div class="toolingOption toolingWithUI toolingDiagramming toolingStaticDiagrams toolingDynamicDiagrams toolingDeploymentDiagrams">
        <a href="https://online.visual-paradigm.com/diagrams/features/c4-model-tool/" target="_blank">Visual Paradigm</a>
    </div>
    <div class="toolingOption toolingWithUI toolingDiagramming toolingStaticDiagrams toolingDynamicDiagrams toolingDeploymentDiagrams">
        <a href="https://github.com/Ferhat67/C4-yEd" target="_blank">yEd</a>
    </div>
</div>

<script>
    $('#toolingOpenSourceFilter, #toolingDiagrammingFilter, #toolingModelBasedFilter, #toolingAsCodeFilter, #toolingWithUIFilter, #toolingRenderingToolIndependentFilter, #toolingStaticDiagramsFilter, #toolingDynamicDiagramsFilter, #toolingDeploymentDiagramsFilter').change(function() {
        filterToolingOptions();
    });

    function filterToolingOptions() {
        var classes = '';

        if ($('#toolingOpenSourceFilter').is(":checked")) {
            classes = classes + '.toolingOpenSource';
        }
        
        if ($('#toolingDiagrammingFilter').is(":checked")) {
            classes = classes + '.toolingDiagramming';
        }
        
        if ($('#toolingModelBasedFilter').is(":checked")) {
            classes = classes + '.toolingModelBased';
        }
        
        if ($('#toolingAsCodeFilter').is(":checked")) {
            classes = classes + '.toolingAsCode';
        }
        
        if ($('#toolingWithUIFilter').is(":checked")) {
            classes = classes + '.toolingWithUI';
        }
        
        if ($('#toolingRenderingToolIndependentFilter').is(":checked")) {
            classes = classes + '.toolingRenderingToolIndependent';
        }
        
        if ($('#toolingStaticDiagramsFilter').is(":checked")) {
            classes = classes + '.toolingStaticDiagrams';
        }
        
        if ($('#toolingDynamicDiagramsFilter').is(":checked")) {
            classes = classes + '.toolingDynamicDiagrams';
        }
        
        if ($('#toolingDeploymentDiagramsFilter').is(":checked")) {
            classes = classes + '.toolingDeploymentDiagrams';
        }
        
        if (classes.length === 0) {
            $('.toolingOption').removeClass('faded');
        } else {
            $('.toolingOption').addClass('faded');
            $('.toolingOption').filter(classes).removeClass('faded');
        }
    }

    filterToolingOptions();
</script>
