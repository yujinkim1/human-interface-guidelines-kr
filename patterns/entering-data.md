---
created-date: 2023-12-17
updated-date: 2024-02-13
supported-platforms:
  - iOS
  - iPadOS
  - macOS
  - tvOS
  - watchOS
  - visionOS
---

# Entering Data

<h2>사용자로부터 정보를 얻어야 할 때, 실수 없이 정보를 제공받을 수 있도록 하는 방법을 설계하세요.</h2>

<div align="center">
  <img alt="patterns-entering-data-intro" src=".attachments/.entering-data/patterns-entering-data-intro@2x.png" width="740"/>
</div>

<br />

사용자가 데이터를 입력하는 것은 상호 작용 방법과 관계없이 지루한 과정일 수 있습니다. 경험을 향상시키려면 다음을 따르세요.

- 가능한 많은 정보를 미리 수집해서 사용자가 입력해야할 데이터의 양을 최소화합니다.
- 사용자가 자신에게 맞는 데이터 입력 방법을 선택할 수 있도록 사용 가능한 모든 입력 방법을 지원하세요.

## Best practices

**가능하면 시스템에서 정보를 가져오세요.**

설정에서 자동으로 수집할 수 있는 정보나 위치, 캘린더 정보처럼 사용자에게 권한을 얻어 사용 할 수 있는 정보는 사용자에게 입력하도록 요청하지 마세요.

<br />

**필요한 사용자 정보를 명확하게 제시하세요.**

텍스트 필드에 "username@company.com"과 같은 프롬프트를 표시하거나 "Email"과 같은 정보를 설명하는 소개 레이블을 제공할 수 있습니다. 또한 적절한 기본값으로 필드를 미리 채울 수도 있으며, 이를 통해 의사 결정을 최소화하고 데이터 입력 속도를 빠르게 할 수 있습니다.

<br />

**민감한 데이터를 필요로 하는 경우 보안 텍스트 필드를 사용하세요.**

일반적으로 각 문자에 대해 작은 Filled circle로 표시하여 사용자가 입력하는 내용을 가립니다. 개발자 가이드라인은 [SecureField](https://developer.apple.com/documentation/SwiftUI/SecureField)를 참고하세요. tvOS에서는 입력하는 숫자를 가려주도록 [digit entry view](./components/digit-entry-view.md)를 구성할 수도 있습니다. 개발자 가이드라인은 [isSecureDigitEntry](https://developer.apple.com/documentation/tvuikit/tvdigitentryviewcontroller/2967056-issecuredigitentry)를 참고하세요.
visionOS에서 시스템 제공 텍스트 필드를 사용하는 경우 시스템은 입력된 데이터를 착용자에게 보여주지만 다른 사람에게는 보여주지 않습니다. 예를 들어, 사용자가 AirPlay를 사용하여 콘텐츠를 스트리밍할 때 보안 텍스트 필드는 자동으로 흐릿해집니다.

<br />

**패스워드 필드를 미리 채우지 마세요.**

항상 사용자에게 패스워드를 입력하거나 생체 인식 또는 키체인 인증을 사용하도록 요청하세요. 자세한 내용은 [Managing accounts](./managing-accounts.md)를 참고하세요.

<br />

**가능하면 텍스트 입력 대신 선택지를 제공하세요.**

키보드를 편리하게 사용할 수 있더라도 데이터를 입력하는 것보다 목록에서 선택하는 것이 일반적으로 더 쉽고 효율적입니다. 의미가 있을 때는 피커, 메뉴 또는 기타 선택 구성 요소를 사용하여 필요한 정보를 쉽게 제공할 수 있도록 하세요.

<br />

**사용자가 정보를 드래그 앤 드롭하거나 붙여넣을 수 있도록 하세요.**

이러한 상호 작용을 지원하면 데이터 입력이 쉬워지고 환경이 시스템과 통합되는 느낌을 줄 수 있습니다.

<br />

**텍스트 필드 값의 유효성을 동적으로 검사하세요.**

사용자는 긴 양식을 작성하다가 실수하면 다시 돌아가서 수정해야 할 때 기분이 안 좋을 수 있습니다.
값을 입력하자마자 확인하고 문제를 감지하는 즉시 피드백을 제공하면 사용자에게 수정할 수 있는 기회를 제공할 수 있습니다. 특히 숫자의 경우 숫자 값만 허용하도록 텍스트 필드를 자동으로 구성하는 숫자 포맷터를 사용하는 것이 좋습니다. 또한 특정 소수 자릿수, 백분율 또는 통화와 같은 특정 방식으로 값을 표시하도록 포맷터를 구성할 수도 있습니다.

<br />

**계속해서 데이터 입력이 필요한 경우 필요한 데이터를 제공해야 한다는 점을 사용자에게 알리세요.**

예를 들어, 양식 뒤에 다음 또는 계속이라는 버튼을 포함하는 경우 사용자가 필요한 데이터를 입력한 후에만 해당 버튼을 사용할 수 있도록 하세요.

## Platform considerations

_iOS, iPadOS, tvOS, visionOS 또는 watchOS에 대한 추가 고려 사항은 없습니다._

### macOS

**확장 도구 설명을 사용하여 필드에서 잘리거나 잘린 텍스트의 전체 버전을 표시하는 것이 좋습니다.**

확장 도구 설명은 일반 도구 설명처럼 동작하며 포인터가 필드 위에 놓일 때 나타납니다. Mac에서 실행되는 iOS 및 iPadOS 앱을 포함하여 macOS에서 실행되는 앱은 확장 툴팁을 사용하여 텍스트 필드가 너무 작아서 표시할 수 없는 경우 사람들이 입력한 전체 데이터를 볼 수 있도록 도울 수 있습니다. 자세한 내용은 [Offering help > macOS, visionOS](https://developer.apple.com/design/human-interface-guidelines/offering-help#macOS-visionOS)를 참조하십시오.

## Resources

### Related

- [Text fields](https://developer.apple.com/design/human-interface-guidelines/text-fields)
- [Virtual keyboards](https://developer.apple.com/design/human-interface-guidelines/virtual-keyboards)
- [Keyboards](../inputs/keyboards.md)

### Developer documentation

- [Input events](https://developer.apple.com/documentation/SwiftUI/Input-events)

### Videos

- [What's new in UIKit](https://developer.apple.com/videos/play/wwdc2021/10059)
