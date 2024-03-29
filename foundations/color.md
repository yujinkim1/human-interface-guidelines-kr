---
create-date: 2023-12-07
update-date: 2023-02-26
supported-platforms:
  - iOS
  - iPadOS
  - macOS
  - tvOS
  - watchOS
  - visionOS
---

# Color

<h2>색상을 구분해서 사용하면 의사소통을 강화하고 브랜드를 연상해내기 쉬우며, 시각적 일관성, 상태 및 피드백을 제공하는데 도움을 줄 수 있습니다.</h2>

시스템은 다양한 배경과 appearance 모드에서 어울리는 색상을 정의하며, 자동으로 생동감과 접근성 설정에 적응할 수 있습니다. 사용자는 시스템 색상에 익숙하며, 이를 사용하면 기기에서 경험이 편안하게 느껴집니다.

또한 앱이나 게임의 시각적 경험을 향상시키고 독특한 개성을 표현하기 위해 사용자 정의 색상을 사용할 수도 있습니다. 다음 가이드라인은 시스템 정의 또는 사용자 정의 색상을 사용하는 방법에 대한 사용자들의 호감을 얻을 수 있도록 도와줄 수 있습니다.

## Best practices

**게임이 아닌 앱에서는 색상을 과하게 사용하지 마세요.**

색상을 과도하게 사용하면 의사소통에 방해가 될 수 있거나 사용자의 주의가 산만해질 수 있습니다. 중요한 정보에만 사용하거나 인터페이스 간의 관계를 표시하기 위해 색상을 사용하는 것을 선호하세요.

<br />

**동일 색상을 다른 의미로 사용하지 마세요.**

전체 인터페이스에서 일관된 색상을 사용하도록 하세요. 상태나 상호 작용과 같은 정보를 전달할 때 색상을 사용합니다. 예를 들어 앱에서 파란색을 사용해서 사용자가 텍스트를 탭하여 더 많은 정보를 볼 수 있음을 나타낼 수 있습니다. 화살표 아이콘처럼 색상에 의존하지 않는 시각 요소를 사용하여 대화형 작업을 전달하는 경우에도 대화형 텍스트에 파란색 이외의 색상을 사용하면 혼란스러울 수 있습니다.

<br />

**앱의 색상이 라이트 모드와 다크 모드에서 모두 잘 보이는지 확인하세요.**

대부분의 플랫폼은 [다크 모드](./dark-mode.md)라고 하는 어두운 Appearance 기능을 제공합니다. 다크 모드는 모든 뷰, 보기, 메뉴 및 컨트롤에 더 어두운 색상 팔레트를 사용하며, 전경색과 배경색을 동적으로 혼합해 생동감을 높여 전경 콘텐츠가 어두운 배경에 비해 더 돋보이도록 할 수 있습니다. 자세한 내용은 [Materials](./materials.md)를 참고하세요. 다크 모드는 visionOS 또는 watchOS에서 사용할 수 없습니다. visionOS는 주변 물체와 색상의 휘도에 자동으로 적응하는 glass라는 요소를 사용합니다. watchOS에서 앱은 일반적으로 어두운 배경을 사용하지만 전체 화면 배경 그라디언트 또는 그래픽을 사용해서 전경 콘텐츠를 지원할 수도 있습니다. 모든 플랫폼에서 시스템 색상은 필요에 따라 라이트 모드 컨텍스트와 다크 모드 컨텍스트를 자동으로 지원합니다. 사용자 정의 색상을 사용하는 경우 두 모드에서 잘 보이도록 제공해야 합니다.

<br />

**다양한 조건에서 앱의 색상 구성표를 테스트하세요.**

예를 들어 밝은 실외 환경이나 어두운 실내 환경에서 앱을 실행할 때 색이 다르게 보일 수 있습니다. visionOS에서 색상은 사용자의 물리적 환경에서 벽이나 물체의 색상과 빛을 반사하는 방식에 따라 다르게 보일 수 있습니다. 대부분의 사례에서 최적의 보기 환경을 제공하기 위해 색상을 조정합니다.

<br />

**다양한 기기에서 앱을 테스트하세요.**

예를 들어 특정 iPhone, iPad, Mac 모델에서 사용할 수 있는 True Tone 디스플레이는 주변광 센서를 사용하여 현재 환경에 맞게 디스플레이의 화이트 포인트를 자동으로 조정합니다. 주로 읽기, 사진, 동영상 및 게임을 지원하는 앱은 화이트 포인트 가변성 스타일을 지정해서 효과를 강화시키거나 약화시킬 수 있습니다. 개발자 가이드라인은 [UIWhitePointAdaptivityStyle](https://developer.apple.com/documentation/uikit/uiwhitepointadaptivitystyle)를 참고하세요. 다양한 디스플레이 설정으로 여러 브랜드의 HD, 4K TV에서 tvOS 앱을 테스트 합니다. Mac에서는 Settings > Display에서 P3 및 표준 RGB(sRGB)와 같은 다양한 색상 프로필을 사용해서 테스트 할 수 있습니다. 자세한 내용은 [Color management](#color-management)를 참고하세요.
