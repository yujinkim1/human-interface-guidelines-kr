---
create-date: 2023-12-07
update-date: 2023-01-09
supported-platforms: iOS, iPadOS, macOS, tvOS, visionOS, watchOS
---

# App icons

<h2> 독특하고 기억에 남는 아이콘은 여러분의 앱이나 게임의 목적과 개성을 전달하며, 사용자가 제품을 한눈에 인식하는 데 도움이 됩니다. </h2>

<div align="center">
  <img alt="app-icons-intro" src=".attachments/.app-icons/foundations-app-icons-intro@2x.png" width="740"/>
</div>

멋진 앱 아이콘은 모든 Apple 플랫폼에서 사용자 경험의 중요한 일부분을 차지하므로 반드시 갖추어야 합니다. 각 플랫폼은 앱 아이콘을 다른 스타일로 정의하고 있어서 모양과 의미의 일관성을 유지하면서 디자인 해야합니다. 각 플랫폼마다 아이콘을 만들 수 있도록 도움을 줄 수 있는 템플릿을 다운로드 하려면 [Apple Design Resources](https://developer.apple.com/design/resources/)를 참고하세요.
다른 유형의 아이콘을 만드는 데 도움이 되는 가이드라인은 [Icons](https://developer.apple.com/design/human-interface-guidelines/icons)를 확인하세요.

## Best practices

**단순함을 채택하세요.**

심플한 아이콘은 사용자가 앱을 이해하기 쉽게 도와줍니다. 앱이나 게임의 본질을 포착하는 개념이나 요소를 찾아 아이콘의 핵심 개념으로 삼고 심플하고 독특한 방식으로 표현하세요. 과한 디테일은 추가하지 마세요. 디테일이 과하거나 크기가 작은 아이콘은 잘 보이지 않을 수 있습니다. 아이콘 전체를 모두 채울 필요는 없으므로 주된 이미지에 중점을 두고 간단한 배경을 선호하는 것이 좋습니다.

<br />

**멀티 플랫폼에서 잘 작동하는 디자인을 만들어 각 플랫폼에서 자연스럽게 느껴지도록 하세요.**

앱이나 게임이 멀티 플랫폼에서 실행되는 경우에는 각 플랫폼에 적합한 스타일로 랜더링하면서 모든 아이콘은 동일한 이미지와 색상을 사용해야 합니다. 예를 들어 iOS, tvOS, watchOS에서 음악 앱 아이콘은 단순화된 그래픽 스타일을 사용해서 빨간색 배경에 하얀색 음표를 표시합니다. macOS에서는 동일한 요소를 표시하면서 음표가 침착된 것처럼 보이도록 그림자를 추가합니다. 마찬가지로 visionOS에서는 동일한 색상 구성과 내용을 사용하지만 장치를 착용한 상태에서 보면 3D 형태로 제공합니다.

<br />

**경험이나 브랜드의 필수 부분인 경우에만 텍스트를 포함하는 것이 좋습니다.**

아이콘 내부 텍스트는 읽기 어렵고, 아이콘 자체를 혼잡하게 만들 수 있으며, 손쉬운 사용이나 지역화를 지원하지 않습니다. 앱 이름이 아이콘 근처에 나타나는 경우 일부 상황에서 아이콘 내부에 이름을 표시한 것과 중복될 수 있습니다. 앱 또는 게임을 인식하는 데 도움이 되도록 이름의 첫 글자와 같은 기억에 남는 것을 사용하는 것은 좋지만, "Watch"나 "Play"와 같은 사용법을 알려주는 비필수 단어나 "New"나 "For visionOS"와 같은 특정 용어를 포함하지 않도록 하세요.

<br />

**사진보다는 그래픽 이미지를 선호하고, 아이콘에서 UI 컴포넌트를 복제하지 마세요.**

사진은 작은 화면에서 보기에 적합하지 않습니다. 사진을 사용하는 대신에 사용자가 주목해야 하는 기능을 강조하는 콘텐츠의 그래픽 표현을 제작하는 것이 좋습니다. 마찬가지로 사용자가 인식할 수 있는 인터페이스가 있는 경우에도 표준 UI 컴포넌트를 단순히 복제하거나 앱 스크린샷을 아이콘에 사용하지 않도록 주의하세요.

<br />

**필요한 경우, 시스템이 Spotlight 검색 결과, 설정 및 알림과 같은 위치에서 표시하는 특정 크기에 대한 아이콘을 최적화하세요.**

iOS, iPadOS 그리고 watchOS의 경우 Xcode를 사용해 1024x1024 px의 에셋으로 모든 크기의 App Store 아이콘을 생성하도록 할 수 있습니다. 또는 일부 또는 모든 개별 아이콘 크기에 대한 에셋을 제공할 수도 있습니다. macOS 및 tvOS의 경우 모든 크기를 제공해야 합니다. visionOS의 경우 1024x1024 픽셀의 단일 에셋을 제공합니다. 앱 아이콘의 자체 버전을 만들 경우 이미지가 모든 크기에서 구별되도록 확인하세요. 세부 정보와 불필요한 기능을 제거하여 이미지를 단순화하고 주요 기능을 과장할 수 있습니다. 이러한 변경을 수행해야 하는 경우에는 이미지가 모든 맥락에서 시각적으로 일관되게 유지되도록 변화를 미세하게 유지하세요.

<div align="center">
  <img alt="app-icon-sizes" src=".attachments/.app-icons/app-icon-sizes@2x.png" width="588"/>
</div>

**아이콘을 풀 블리드 정사각형 이미지로 디자인하세요.**

대부분의 플랫폼에서 시스템은 아이콘 모서리를 플랫폼에 맞게 자동으로 조절된 마스크를 적용합니다. 예를 들어서 visionOS 및 watchOS에서는 자동으로 원형 마스크를 적용합니다. Mac Catalyst로 생성된 앱의 경우 시스템이 둥근 직사각형 모양을 아이콘에 자동으로 적용하지만, macOS 앱 아이콘은 올바른 둥근 형태로 만들어야 합니다. 자세한 내용은 [macOS](/foundations/app-icons.md/#macOS)를 참조하세요. visionOS 및 tvOS에서 레이어로 구성된 앱 아이콘의 경우 풀 블리드 콘텐츠가 하단 레이어에 가장 적합합니다. 각 플랫폼에 대한 앱 아이콘을 생성하는 데 도움이 되는 제작용 템플릿은 [Apple Design Resources](https://developer.apple.com/design/resources/)에서 제공됩니다.

> 풀 블리드(Full-bleed): 테두리 또는 여백이 없이 이미지가 모든 영역을 채우는 것.

<br />

**대체 앱 아이콘을 제공하는 것을 고려하세요.**

iOS, iPadOS, tvOS, visionOS에서는 사용자가 앱이나 게임과의 연결을 강화하고 경험을 향상시킬 수 있는 아이콘의 대체 버전을 선택할 수 있습니다. 예를 들어, 스포츠 앱은 다른 팀을 나타내는 다양한 아이콘을 제공할 수 있습니다. 디자인한 각 대체 앱 아이콘이 콘텐츠 및 경험과 밀접하게 관련되어 있도록 하고, 사용자가 다른 앱의 아이콘으로 오인할 수 있는 버전은 만들지 않도록 주의하세요. 사용자가 대체 아이콘으로 전환하려면 앱의 설정으로 이동할 수 있습니다.

> ***NOTES***
>
> 기본 앱 아이콘과 마찬가지로 대체 앱 아이콘도 앱 리뷰의 대상이며 [App Store Review Guidelines](https://developer.apple.com/app-store/review/guidelines/#design)를 준수해야 합니다.

<br />

**Apple 하드웨어 제품의 복제품을 사용하지 마세요.**

Apple의 제품은 저작권이 있으며 앱 아이콘으로 재현될 수 없습니다.

<br />

## Platform considerations

### iOS, iPadOS

**설정에 나타나는 아이콘에 오버레이나 테두리를 추가하지 마세요.** 

iOS는 모든 아이콘에 1px 굵기를 자동으로 추가하여 설정에서 잘 보이게 합니다.

### macOS

macOS에서 앱 아이콘은 둥근 직사각형 모양, 전방 투영, 수평 위치 및 균일한 그림자와 같은 일련의 시각적 속성을 공유합니다. macOS 디자인 언어를 기반으로 한 이러한 특성들은 macOS에서 사용자가 기대하는 생동감 있는 렌더링 스타일을 보여주면서 조화로운 사용자 경험을 제공합니다.

**사용자가 앱을 어떻게 사용하는지 전달하기 위해 익숙한 도구를 묘사하는 것을 고려하세요.**

앱의 목적에 맥락을 부여하기 위해 아이콘 배경을 사용하여 도구의 환경이나 해당 도구가 영향을 미치는 항목을 묘사할 수 있습니다. 예를 들어 TextEdit 아이콘은 기계 연필과 선이 그어진 종이 시트를 결합하여 실용적인 글쓰기 경험을 시사합니다. 도구의 상세하고 현실적인 이미지를 만든 후에는 이를 배경 위로 부드럽게 떠오르게 하고 아이콘 경계를 약간 벗어나게 하는 것이 종종 효과적입니다. 이렇게 하는 경우 도구가 배경과 시각적으로 통일되고 둥근 직사각형 모양을 압도하지 않도록 주의하십시오.

<div align="center">
  <img alt="app-icon-familiar-tool" src=".attachments/.app-icons/app-icon-familiar-tool@2x.png" width="294"/>
</div>

**앱 아이콘에 실제 물체를 묘사한다면, 물리적인 물질로 만들어진 것처럼 보이도록 하고 실제로 질량이 있는 것처럼 만드는 것이 좋습니다.**

객체의 무게와 느낌을 전달하기 위해 천, 유리, 종이, 금속과 같은 물질의 특성을 묘사하는 것을 고려해보세요. 예를 들어서 Xcode 앱 아이콘의 망치는 강철로된 망치머리와 폴리머 손잡이로 구성되어 있습니다.

<div align="center">
  <img alt="app-icon-realistic-materials" src=".attachments/.app-icons/app-icon-realistic-materials@2x.png" width="294"/>
</div>

**앱 아이콘 디자인 템플릿에서 그림자 효과를 사용하세요.**

이 그림자 효과는 시스템에서 정의한 macOS 아이콘의 시각적 속성 중 하나입니다. 이를 통해 앱 아이콘이 다른 macOS 아이콘과 조화롭게 어우러지며 macOS 플랫폼의 일관된 시각적 통일성을 유지하는 데 도움이 됩니다.

<br />

**내부 그림자와 강조를 사용하여 정의와 현실감을 더해보세요.**

예를 들어, Mail 앱 아이콘은 봉투에 실감을 주기 위해 그림자와 강조를 모두 사용하며 덮개가 약간 열려있는 것처럼 보입니다. TextEdit나 Xcode와 같이 배경 위에 떠다니는 도구를 포함하는 아이콘에서 내부 그림자는 깊이를 강화하고 도구가 현실적으로 보이게 할 수 있습니다. 아이콘에 빛이 오는 방향을 나타내는 내부 그림자와 강조를 사용하고, 이 빛은 아이콘 위에서 약간 아래쪽으로 기울여진 상태로 위치해 있다고 가정하세요.

**다른 형태를 시사하는 윤곽을 정의하지 않도록 주의하세요.**

드물게 기본 앱 아이콘 모양을 미세하게 조정하고 싶을 수 있지만, 이렇게 하는 것은 macOS에 속하지 않는 아이콘을 만들 가능성이 있습니다. 모양을 수정해야 하는 경우, 계속해서 둥근 직사각형 실루엣을 나타내는 섬세한 조정을 선호하세요.

<div align="center">
  <img alt="app-icon-consistent-shape" src=".attachments/.app-icons/app-icon-consistent-shape@2x.png" width="294"/>
</div>

**기본 컨텐츠를 아이콘 그리드 바운딩 박스 내에 유지하세요. 모든 컨텐츠를 외부 바운딩 박스 내에 유지하세요.**

아이콘의 주요 컨텐츠가 아이콘 그리드 바운딩 박스를 벗어나면 보기 어색할 수 있습니다. 아이콘에 도구를 오버레이하는 경우, 도구의 상단 가장자리를 외부 바운딩 박스와 정렬하고 하단 가장자리를 내부 바운딩 박스와 정렬하는 것이 잘 작동합니다. 그리드를 사용하여 아이콘 내에서 항목을 배치하고 중앙에 정렬된 원 같은 내부 요소가 시스템의 다른 아이콘과 일관된 크기를 사용하는지 확인할 수 있습니다.

<div align="center">
  <img alt="app-icon-layout-guides" src=".attachments/.app-icons/app-icon-layout-guides@2x.png" width="294"/>
</div>

### tvOS

### visonOS
