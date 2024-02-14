---
created-date: 2023-12-16
updated-date: 2024-02-15
surpported-platforms:
  - iOS
  - iPadOS
  - macOS
  - tvOS
  - watchOS
  - visionOS
---

# Managing accounts

<h2>계정은 사람들이 콘텐츠에 액세스하고 개인 정보를 추적하는 간편한 방법이 될 수 있습니다.</h2>

<div align="center">
  <img alt="patterns-managing-accounts-intro" src=".attachments/.managing-accounts/patterns-managing-accounts-intro@2x.png" width="740" />
</div>

<br />

계정이 필요한 경우에만 생성하는 것을 권장하고, 그렇지 않은 경우 사용자가 계정이 없어도 앱이나 게임을 즐길 수 있도록 하세요. 계정이 필요한 경우 [Sign in with Apple](https://developer.apple.com/design/human-interface-guidelines/sign-in-with-apple)을 사용해서 사용자가 신뢰할 수 있는 일관된 로그인 경험과 여러 계정과 인증 방법을 기억할 필요가 없는 간편함을 제공하는 것이 좋습니다.

## Best practices

**계정을 생성하면 좋은 점과 가입 방법을 설명하세요.**

앱이나 게임에서 계정이 필요한 경우, 해당 요구 사항과 혜택에 대한 간단하고 친근한 설명을 작성하고 이 메시지를 로그인 화면에 표시하세요.

<br />

**가능한 한 오랫동안 로그인을 지연하세요.**

사용자는 로그인을 강제로 해야 하는 경우 종종 앱을 포기합니다. 이러한 상황을 피하기 위해 사용자에게 앱이나 게임이 무엇을 하는지 먼저 감을 잡을 기회를 제공하세요.(예: 쇼핑 앱은 사람들이 원하는 만큼 둘러보게 하고, 실제로 구매하려고 할 때만 로그인을 요구)

<br />

**iOS, iPadOS, macOS, visionOS 앱에서 Sign in with Apple을 사용하지 않는 경우 패스키를 사용하는 것이 좋습니다.**

패스키를 사용하면 계정 생성과 인증이 간단해지며, 사용자가 비밀번호를 생성하거나 입력할 필요가 없어집니다. 앱이 passkey를 지원하는 경우, 새 계정을 만들거나 기존 계정에 로그인할 때 사용자 이름만 제공하면 됩니다. 자세한 내용은 [Supporting passkeys](https://developer.apple.com/documentation/authenticationservices/public-private_key_authentication/supporting_passkeys)를 참고하세요. 인증에 계속해서 비밀번호를 사용해야 하는 경우, 이중 인증을 요구함으로써 보안을 강화하세요. 자세한 내용은 [Securing Logins with iCloud Keychain Verification Codes](https://developer.apple.com/documentation/authenticationservices/securing_logins_with_icloud_keychain_verification_codes)를 참고하세요.

<br />

**항상 제공하는 인증 방법을 식별화하세요.**

예를 들어, Face ID로 앱에 로그인할 수 있는 버튼을 표시하는 경우 "Face ID로 로그인"과 같은 구문을 사용하세요. "로그인"과 같은 일반적인 구문 대신에 사용 가능한 인증 방법만 언급하세요.

<br />

**일반적으로 생체 인증을 사용하는 앱 설정을 제공하지 마세요.**

사용자는 생체 인증을 시스템에서만 활성화하므로 앱 내 설정에서 이를 제시하는 것은 중복되고 혼동을 일으킬 수 있습니다.

<br />

**계정 인증을 나타내는 용어로 "passcode"를 사용하지 마세요.**

사용자는 기기를 잠금 해제하거나 Apple 서비스에 로그인하기 위해 passcode를 만듭니다. 인터페이스에서 이 용어를 사용하면 사용자가 앱이나 게임에서 자신의 passcode를 재사용하라는 것으로 오해할 수 있습니다.

## Deleting accounts

앱이나 게임 내에서 계정을 생성하도록 유도하는 경우 계정을 비활성화하는 것뿐만 아니라 삭제도 할 수 있도록 제공해야 합니다. 아래 내용을 준수하는 것 외에도 계정 삭제 및 잊혀질 권리와 관련된 지역법을 준수해야 합니다.

> **Important**
> 
> 법률에 따라 앱에서 계정 또는 사용자 정보를 유지 및 관리하거나 특정 계정 삭제 프로세스를 수행해야 하는 경우 해당 사용자에게 이러한 상황을 명확하게 전달해야 합니다.

**앱 또는 게임 내에서 계정을 삭제하는 명확한 방법을 제공하세요.**

사용자가 계정 삭제할 수 없는 경우 사용자가 계정을 삭제할 수 있는 웹페이지로 직접 연결되는 링크로 제공해야 합니다. 링크는 쉽게 찾을 수 있도록 하세요.

<br />

**웹페이지에서 계정 삭제가 가능한지에 대한 여부와 관계없이 계정 삭제 기능을 제공하세요.**

계정 삭제 프로세스를 너무 길거나 복잡하게 설계하지 마세요.

<br />

**사용자의 계정이 나중에 삭제되도록 예약하는 것도 좋습니다.**

사용자가 계정은 삭제하고 싶지만 나머지 서비스를 제공받고 싶거나 구독 잔여 기간이 자동 갱신되기 이전까지 계정을 삭제하고 싶지 않을 수 있습니다. 이러한 방법을 제공할 경우 즉시 삭제하는 옵션도 제공하세요.

<br />

**계정 삭제가 완료되는 시점과 완료 후 사용자에게 알리세요.**

계정을 완전히 삭제하는 데 시간이 걸릴 수 있으므로 계정 삭제 프로세스 상태를 사용자에게 알리는 것이 중요합니다.

<br />

**앱에서 인앱 결제를 지원하는 경우 사용자가 계정을 삭제할 때 결제 정보 취소에 대해 고지하세요.**

예를 들어 다음과 같이 사용자에게 고지해야할 수 있습니다:

- 자동 갱신 구독에 대한 청구는 계정 삭제 여부와 관계없이 사용자가 구독을 취소할 때까지 Apple 계정으로 계속 진행됩니다.
- 계정을 삭제한 후에는 구독을 취소하거나 환불을 요청해야 합니다.

사용자가 이러한 과정을 이해하도록 고지하는 것 외에도 구독을 취소하고 구매내역을 관리하는 방법을 설명하는 정보를 제공하는 것도 중요합니다. 자세한 내용은 [In-App Purchase](https://developer.apple.com/in-app-purchase/)를 참고하세요.

## TV provider accounts

TV 제공업체는 사용자가 시스템 수준에서 계정에 로그인할 수 있도록 허용하므로 앱별로 인증할 필요는 없습니다.
TV 제공업체 앱에서 사용자가 로그인해야 하는 경우 TV 제공업체가 제공하는 인증 방법을 사용하세요.

**사용자가 시스템 수준에서 로그인할 때 로그아웃 옵션은 표시하지 마세요.**

앱에 로그아웃 옵션을 포함해야 하는 경우 이를 호출하면 사용자가 Settings > TV provider 메뉴로 이동하여 계정에서 로그아웃하라는 메시지를 표시하세요.

<br />

**개인 정보 보호 설정을 조정해 로그아웃하도록 사용자에게 유도하지 마세요.**

Settings > Privacy > TV provider control 기능은 로그아웃 기능이 아닙니다. 이러한 설정은 사용자가 TV 제공업체 계정에 접근할 수 있는 앱을 관리하는 데 도움을 주는 것입니다.

## Platform considerations

_iOS, iPadOS, macOS, watchOS, visionOS에 대한 추가 고려사항은 없습니다._

### tvOS

대부분의 사용자는 키보드가 아닌 리모컨을 사용해 Apple TV와 상호 작용하므로 가능하면 최소한의 정보만 요구하세요.

**사용자가 다른 기기를 사용해서 로그인하거나 인증할 수 있도록 하는 것이 좋습니다.**

앱의 연결된 도메인을 구성하면 Apple TV가 다른 기기와 연동되어 Sign in with Apple을 포함한 로그인 certificate를 안전하게 제안할 수 있습니다. 개발자 가이드라인은 [Configuring an associated domain](https://developer.apple.com/documentation/Xcode/configuring-an-associated-domain)를 참고하세요.

<br />

**사용자가 공유 계정에 로그인한 경우 현재 사용자의 프로필을 선택하도록 요청하지 마세요.**

tvOS 16 이상에서는 앱이 모든 사용자와 사용자 인증 정보를 공유하면서 각 개인의 프로필과 사용자 데이터를 별도로 저장합니다. 앱에서 각 사용자에게 공유 계정에 별도로 로그인하도록 요청하지 않고 현재 사용자의 프로필을 자동으로 사용할 수 있습니다. 개발자 가이드라인은 [kSecUseUserIndependentKeychain](https://developer.apple.com/documentation/security/ksecuseuserindependentkeychain)과[User Management Entitlement](https://developer.apple.com/documentation/bundleresources/entitlements/com_apple_developer_user-management)를 참고하세요.

<br />

### watchOS

iCloud 동기화를 사용해서 키체인에 대한 접근을 제공하여 사용자 이름과 암호를 자동으로 채우고 앱 설정을 유지할 수 있도록 하세요.

## Resources

### Related

- [Onboarding](./onboarding.md)
- [Sign in with Apple](../technologies/sign-in-with-apple.md)

### Developer Documentation

- [Supporting passkeys](https://developer.apple.com/documentation/authenticationservices/public-private_key_authentication/supporting_passkeys)

### Videos

- [Move beyond passwords](https://developer.apple.com/videos/play/wwdc2021/10106)
- [Discover account-driven User Enrollment](https://developer.apple.com/videos/play/wwdc2021/10136)
- [Simplify sign in for your tvOS apps](https://developer.apple.com/videos/play/wwdc2021/10279)
