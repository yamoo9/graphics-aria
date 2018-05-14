# WAI-ARIA Graphics Module 1.0

W3C 표준 입후보안(<abbr title="Candidate Recommendation">CR</abbr>) - 2018.03.29<br>
[WAI-ARIA 그래픽 모듈 (Graphics Module)](https://www.w3.org/TR/graphics-aria-1.0/)
문서에서 제작 과정에 필요한 내용을 발췌하여 일부 번역(의역)을 진행했습니다.

### 목차

각 섹션 링크를 통해 번역된 내용을 확인할 수 있습니다.

1. [WAI-ARIA 그래픽 모듈](https://github.com/yamoo9/graphics-aria/wiki)
1. [그래픽 역할(Roles)](https://github.com/yamoo9/graphics-aria/wiki/%EA%B7%B8%EB%9E%98%ED%94%BD-%EC%97%AD%ED%95%A0-(Graphics-Roles))
    - [그래픽 문서(Document)](https://github.com/yamoo9/graphics-aria/wiki/%EA%B7%B8%EB%9E%98%ED%94%BD-%EB%AC%B8%EC%84%9C-(graphics-document)-%EC%97%AD%ED%95%A0)
    - [그래픽 객체(Object)](https://github.com/yamoo9/graphics-aria/wiki/%EA%B7%B8%EB%9E%98%ED%94%BD-%EA%B0%9D%EC%B2%B4(Graphic-Object)-%EC%97%AD%ED%95%A0)
    - [그래픽 심볼(Symbol)](https://github.com/yamoo9/graphics-aria/wiki/%EA%B7%B8%EB%9E%98%ED%94%BD-%EC%8B%AC%EB%B3%BC(Graphic-Symbol)-%EC%97%AD%ED%95%A0)
    - [그외 다른 역할(Other Roles)](https://github.com/yamoo9/graphics-aria/wiki/%EA%B7%B8%EC%99%B8-%EB%8B%A4%EB%A5%B8-%EC%97%AD%ED%95%A0(Other-Roles))
1. [상태(States)와 속성(Properties)](https://github.com/yamoo9/graphics-aria/wiki/%EC%83%81%ED%83%9C(States)%EC%99%80-%EC%86%8D%EC%84%B1(Properties))

<br>

---

<br>

## SVG 그래픽 / 접근성

SVG 그래픽에 대한 이해를 돕고, 사용하는 방법에 대해 안내합니다.
나아가 그래픽에 접근성을 고려하는 방법을 다뤄봅니다.

1. [SVG 그래픽](SVG/README.md)
1. [SVG 접근성](SVG/a11y.md)

<br>

## W3C 접근성 API 매핑(Mapping)

매핑 API는 <u>웹 개발자가 아닌 브라우저, 보조 기술 개발자가 참고해야 할 문서</u>입니다.

### [Graphics Accessibility API Mappings (W3C 표준 입후보안 - 2018.04.19)](https://www.w3.org/TR/graphics-aam-1.0/)

그래픽 접근성 API 매핑은 유저 에이전트(UA)가 WAI-ARIA 그래픽 모듈 [GRAPHICS-ARIA-1.0](https://www.w3.org/TR/graphics-aria-1.0/) 마크업을 [플랫폼 마크업 접근성 API](https://www.w3.org/TR/svg-aam-1.0/#dfn-accessibility-api)에 매핑(Mapping: A 집합에 속하는 요소와 B 집합에 속하는 요소 사이 1:1 대응)하는 방법을 정의합니다.

[SVG](https://www.w3.org/TR/graphics-aam-1.0/#bib-SVG) 또는 [HTML5.2](https://www.w3.org/TR/graphics-aam-1.0/#bib-HTML52) 용으로 작성된 것과 같은 그래픽의 접근성을 지원할 수 있도록 유저 에이전트에서 접근성을 담당하는 **유저 에이전트 개발자를 위한** 것입니다.

유저 에이전트에서 이 명세를 구현하면 제작자는 보편적인 그래픽 의미 체계를 보조 기술로 전달함으로써 보다 접근하기 쉬운 그래픽을 생성 할 수 있습니다. WAI-ARIA 그래픽 모듈 [GRAPHICS-ARIA-1.0](https://www.w3.org/TR/graphics-aria-1.0/)에 정의된 역할에 대한 접근성 API 매핑 가이드를 제공합니다.

그래픽 접근성 API 매핑은 WAI-ARIA 개요에 설명 된 WAI-ARIA 제품군의 일부입니다.

### [SVG Accessibility API Mappings (W3C 초안 - 2018.05.10)](https://www.w3.org/TR/svg-aam-1.0/)

SVG 접근성 API 매핑은 유저 에이전트가 [SVG2](https://www.w3.org/TR/svg-aam-1.0/#bib-SVG2) 마크업을 플랫폼 마크업 접근성 API에 매핑하는 방법을 정의합니다. 유저 에이전트에서 SVG 접근성을 담당하는 **SVG 유저 에이전트 개발자를 위한** 것입니다.

이 사양은 SVG 제작자가 차트(Chart), 그래프(Graph) 및 기타 도면(drawings)을 포함하여 접근 가능한 리치 애플리케이션(RIA)을 만들 수 있도록 합니다. 이것은 [Core Accessibility API Mappings 1.1](http://www.w3.org/TR/core-aam-1.1/) (CORE-AAM) [[CORE-AAM](https://www.w3.org/TR/svg-aam-1.0/#bib-CORE-AAM)]과 [Accessible Name and Description: Computation and API Mappings 1.1](http://www.w3.org/TR/accname-1.1/) (ACCNAME-AAM) [[ACCNAME-AAM](https://www.w3.org/TR/svg-aam-1.0/#bib-ACCNAME-AAM)]을 유저 에이전트에 확장하기에 가능합니다.

이러한 핵심 매핑을 활용하고 SVG 유저 에이전트가 [WAI-ARIA](http://www.w3.org/TR/wai-aria-1.1/) [[WAI-ARIA](https://www.w3.org/TR/svg-aam-1.0/#bib-WAI-ARIA)]를 통해 웹 컨텐츠에서 제공되는 키보드 포커스와 역할([role](https://www.w3.org/TR/svg-aam-1.0/#dfn-role)), 상태([state](https://www.w3.org/TR/svg-aam-1.0/#dfn-state)) 및 속성([property](https://www.w3.org/TR/svg-aam-1.0/#dfn-property)) 속성에 응답해야 하는 방법을 정의하는 SVG 관련 가이드를 제공합니다. 또한 SVG-AAM은 ACCNAME-AAM이 플랫폼 접근성 API에 의해 공개된 접근 가능한 이름과 설명 정보를 계산하는데 사용되는 표준 SVG 기능을 사용하도록 조정합니다.

SVG-AAM은 [WAI-ARIA 개요](http://www.w3.org/WAI/intro/aria.php)에 설명된 WAI-ARIA 제품군의 일부입니다.

<br>

## 플랫폼(운영체제) 접근성 API

운영체제 및 기타 플랫폼은 [객체](https://www.w3.org/TR/graphics-aam-1.0/#dfn-object) 및 [이벤트](https://www.w3.org/TR/graphics-aam-1.0/#dfn-event)에 대한 정보를 [보조 기술](https://www.w3.org/TR/graphics-aam-1.0/#dfn-assistive-technology)에 공개하는 일련의 인터페이스를 제공합니다. 보조 기술은 이러한 인터페이스를 사용하여 [위젯](https://www.w3.org/TR/graphics-aam-1.0/#dfn-widget)에 대한 정보를 얻고 인터랙션 합니다.

- [MSAA(MicroSoft Active Accessibility)](https://msdn.microsoft.com/en-us/library/ms697270(VS.85).aspx)
- [UI-AUTOMATION(Microsoft User Interface Automation)](https://msdn.microsoft.com/en-us/library/ee684013%28VS.85%29.aspx)
- [UIA-EXPRESS(MSAA with UIA Express)](https://msdn.microsoft.com/en-us/library/windows/desktop/dd561898(v=vs.85).aspx)
- [AXAPI(Mac OS X Accessibility Protocol)](https://developer.apple.com/documentation/appkit/accessibility/nsaccessibility)
- [ATK(Linux/Unix Accessibility Toolkit)](https://developer.gnome.org/atk/unstable/)
- [AT-SPI(Assistive Technology Service Provider Interface)](https://developer.gnome.org/libatspi/stable/)
- [IAccessible2](https://wiki.linuxfoundation.org/accessibility/iaccessible2/start)
