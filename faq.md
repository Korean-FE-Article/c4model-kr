---
layout: default
title: 자주 묻는 질문
nav_order: 20
permalink: /faq
---

# 자주 묻는 질문

## C4 모델이 만들어지게 된 배경은 무엇인가요?

C4 모델은 소프트웨어 개발자이자 아키텍트로 일하면서 소프트웨어 아키텍처를 가르치기 시작한 [Simon Brown](http://simonbrown.je)이 개발했습니다. Simon의 교육 과정 중 일부는 설계 실습으로 이루어지며, 여러 사람에게 몇 가지 요구 사항을 제시하고 설계를 수행하도록 한 후, 그 설계를 표현하는 다이어그램을 그리는 것이었습니다.

설계에 초점을 맞춘 실습이었지만, 대부분의 사람이 다양한 다이어그램을 통해 아이디어를 시각화하는 데 어려움을 겪는다는 것을 확실히 확인할 수 있었습니다. 본질적으로 C4 모델은 Simon이 소프트웨어 아키텍처를 시각화하는 방식을 공식화한 것으로, 수년에 걸쳐 발전해 왔습니다.

정확한 날짜를 특정하기는 어렵지만, C4 모델의 뿌리는 2006~2009년으로 거슬러 올라갈 수 있습니다. 2010년 초에 다이어그램 유형("컨텍스트", "컨테이너", "컴포넌트", "클래스")이 명명되었고, 2011년 초에 "C4"라는 이름이 처음 사용되었습니다. 네 번째 다이어그램 유형은 2015~2016년에 "클래스"에서 "코드"로 이름이 변경되었습니다.

## C4 모델은 어디에서 영감을 받았나요?

C4 모델은 애자일 운동의 영향을 받은 팀들이 [통합 모델링 언어(Unified Modeling Language, UML)](https://en.wikipedia.org/wiki/Unified_Modeling_Language)를 사용하여 소프트웨어 아키텍처를 문서화하는 데 그다지 적극적이지 않았고, 다이어그램을 작성하는 것조차 꺼렸던 시기에 만들어졌습니다. 그럼에도 불구하고 C4 모델은 UML과 [소프트웨어 아키텍처를 위한 4+1 모델](https://en.wikipedia.org/wiki/4%2B1_architectural_view_model)에서 영감을 받았습니다. 요약하자면, C4 모델은 기본 개념을 단순화한 버전으로, (1) 소프트웨어 개발자가 소프트웨어 시스템의 작동 방식을 더 쉽게 설명하고 이해할 수 있도록 하고, (2) 소프트웨어 아키텍처 모델/설명과 소스 코드 간의 차이를 최소화하기 위해 설계되었습니다.

## C4 모델은 퇴보 아닌가요? 왜 UML을 다시 만드는 건가요? 왜 그냥 UML을 쓰지 않는 건가요?

C4 모델을 발전으로 볼지, 퇴보로 볼지는 각자의 상황에 따라 다릅니다. UML(또는 SysML, ArchiMate 등)을 사용하고 있고 잘 작동한다면 계속 사용하세요. 안타깝게도 UML 사용률은 감소하는 추세이며, 많은 팀이 다시 임시방편으로 상자와 선을 이용한 다이어그램을 사용하는 방식으로 회귀했습니다. 이러한 팀 중 다수가 여러 가지 이유로 UML을 사용하고 싶어하지 않는다는 점을 고려하면, C4 모델은 소프트웨어 아키텍처를 전달하는 방식에 구조와 원칙을 도입하는 데 도움이 됩니다. 많은 팀에게 C4 모델만으로도 충분합니다. 그리고 어떤 팀에게는 UML로 가는 디딤돌이 될 수도 있습니다.

## C4 모델이 비즈니스 프로세스, 워크플로, 상태 머신, 도메인 모델, 데이터 모델 등을 다루지 않는 이유는 무엇인가요?

C4 모델은 소프트웨어 시스템을 구성하는 정적 구조에 초점을 둡니다. 각 구조는 다양한 추상화 수준에서 표현됩니다. 다른 측면을 설명해야 하는 경우 UML 다이어그램, BPML 다이어그램, ArchiMate 다이어그램, 개체 관계 다이어그램 등을 사용하여 C4 다이어그램을 보완할 수 있습니다.

## C4 모델은 설계 프로세스나 팀 구조를 의미하나요?

팀의 설계 프로세스가 C4 모델 계층 구조의 수준을 따라야 한다는 오해가 흔히 있습니다. 팀 내 여러 구성원이 각기 다른 수준의 다이어그램을 담당하는 경우도 있습니다. 예를 들어, 비즈니스 분석가는 시스템 컨텍스트 다이어그램을 작성하고, 아키텍트는 컨테이너 다이어그램을 작성하며, 개발자는 나머지 세부 수준을 관리합니다.

물론 C4 모델을 이런 방식으로 사용할 수는 있지만, 이는 의도되거나 권장되는 사용 패턴이 아닙니다. C4 모델은 다양한 추상화 수준에서 소프트웨어 시스템을 설명하는 방식일 뿐이며, 소프트웨어 제공 프로세스와는 아무런 관련이 없습니다.

## 라이브러리, 프레임워크, SDK를 설명하는데 C4를 사용하시나요?

C4 모델은 실제로 다양한 추상화 수준에서 소프트웨어 시스템을 모델링하도록 설계되었습니다. 라이브러리, 프레임워크 또는 SDK를 문서화하려면 UML과 같은 것을 사용하는 것이 더 나을 수 있습니다. 또는 C4 모델을 사용하여 프레임워크, 라이브러리 또는 SDK의 사용 사례를 설명할 수도 있습니다. 소프트웨어 시스템의 어떤 부분이 맞춤형인지, 어떤 부분이 제공되는지 색상으로 구분하는 것도 좋은 방법입니다.

## C4 모델은 보편적으로 적용 가능한가요?

C4 모델은 맞춤형 소프트웨어 시스템을 설명, 문서화 및 다이어그램으로 표현하는 데 도움을 주기 위해 설계되었습니다. 이러한 관점에서 C4 모델은 다양한 프로그래밍 언어로 구축되고 다양한 플랫폼(온프레미스 또는 클라우드)에 배포되는 다양한 소프트웨어 아키텍처(모놀리식 또는 분산형)를 설명하는 데 사용될 수 있습니다.

C4 모델에 덜 적합한 솔루션으로는 임베디드 시스템/펌웨어, 그리고 맞춤형 개발보다는 대규모 맞춤 설정에 의존하는 솔루션(예: SAP, Salesforce)이 있습니다. 이러한 솔루션을 사용하더라도 시스템 컨텍스트 및 컨테이너 다이어그램이 여전히 유용할 수 있습니다.

## C4 모델은 확장 가능한가요?

예제 다이어그램은 몇 개의 상자와 화살표만으로 간단하게 만들어졌습니다. 하지만, 실제 소프트웨어 시스템은 6개가 아니라 600개의 컴포넌트를 가질 수 있습니다. 이럴 때도 C4 모델을 사용할 수 있을까요? 핵심은 어떤 도구를 선택하느냐입니다. 도구에 따라 작업이 쉬워질 수도, 어려워질 수도 있습니다.

비교적 작은 소프트웨어 시스템이라도 전체 내용을 하나의 다이어그램에 담으려는 유혹이 큽니다. 예를 들어 웹 애플리케이션이 있다면, 해당 웹 애플리케이션을 구성하는 모든 컴포넌트를 보여주는 단일 컴포넌트 다이어그램을 만드는 것이 논리적으로 보입니다. 하지만 소프트웨어 시스템이 실제로 그렇게 작지 않다면 다이어그램 캔버스 공간이 부족하거나, 수많은 선이 겹쳐 어수선하게 보이는 레이아웃이 되는 것을 피하기 어려울 수 있습니다. 더 큰 다이어그램 캔버스를 사용하는 것이 도움이 될 수도 있지만, 큰 다이어그램은 인지 부하가 ​​너무 커서 해석하고 이해하기 어렵습니다. 아무도 다이어그램을 이해하지 못하면 아무도 다이어그램을 보지 않을 것입니다.

대신, 그 복잡한 하나의 다이어그램을 여러 개의 더 단순한 다이어그램으로 나누는 것을 두려워하지 마세요. 각 다이어그램은 특정 비즈니스 영역, 기능 영역, 기능 그룹, 제한된 컨텍스트, 사용 사례, 사용자 상호 작용, 기능 세트 등에 초점을 맞춥니다. 중요한 것은 각각의 개별 다이어그램이 동일한 추상화 수준에서 동일한 전체 내용의 다른 부분을 전달하는지 확인하는 것입니다.

다음은 여러 개의 마이크로서비스로 구성된 소프트웨어 시스템을 보여주는 컨테이너 다이어그램의 예입니다.

[![]({{ site.baseurl }}/images/scale-1.png)]({{ site.baseurl }}/images/scale-1.png)

이 다이어그램은 현재로서는 잘 작동하지만, 서비스를 더 추가할수록 복잡해질 것입니다. 다른 방법으로, 8개의 서비스를 보여주는 하나의 다이어그램을 만드는 대신, 각각 하나의 서비스에 집중하고 가장 가까운 유입(인바운드) 및 유출(아웃바운드) 종속성을 보여주는 8개의 다이어그램을 만들 수 있습니다.

| [![]({{ site.baseurl }}/images/scale-2.png)]({{ site.baseurl }}/images/scale-2.png) | [![]({{ site.baseurl }}/images/scale-3.png)]({{ site.baseurl }}/images/scale-3.png) | [![]({{ site.baseurl }}/images/scale-4.png)]({{ site.baseurl }}/images/scale-4.png) |
| ----------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------- |
| Service 1                                                                           | Service 2                                                                           | Service 3                                                                           |

이 작업은 다이어그래밍 도구에서는 어렵지만 모델링 도구에서는 간단합니다. 자세한 내용은 [다이어그래밍과 모델링]({{ site.baseurl }}/tooling#diagramming-vs-modelling)을 참고하세요. 여기서 단점은 "큰 그림"을 놓칠 수 있다는 것입니다. 따라서 기존의 "상자와 선" 다이어그램처럼 장황하지 않은 다른 시각화 방법을 만드는 것이 또 다른 옵션일 수 있습니다. 다시 말하지만, 모델링 도구를 사용하고 소프트웨어 아키텍처 모델을 다양한 방식으로 시각화할 수 있는 데이터 구조로 생각하면 비교적 간단합니다.

|-|-|
|[![]({{ site.baseurl }}/images/scale-5.png)]({{ site.baseurl }}/images/scale-5.png)|[![]({{ site.baseurl }}/images/scale-6.png)]({{ site.baseurl }}/images/scale-6.png)|
