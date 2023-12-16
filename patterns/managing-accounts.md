---
description: 계정은 사람들이 콘텐츠에 액세스하고 개인 정보를 추적하는 간편한 방법이 될 수 있습니다.
create-date: 2023-12-16
update-date: 2023-12-16
---

# Managing accounts

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
