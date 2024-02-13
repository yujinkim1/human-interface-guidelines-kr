---
create-date: 2023-12-15
update-date: 2023-02-13
supported-platforms:
  - iOS
  - iPadOS
  - macOS
  - tvOS
  - watchOS
  - visionOS
---

# Loading

<h2>콘텐츠가 로드되는 동안 사용자가 앱이나 게임이 느려지거나 멈췄다고 생각할 수 있는 빈 화면이나 정적인 콘텐츠를 표시하지 마세요.</h2>

<div align="center">
  <img alt="patterns-loading-intro" src=".attachments/.loading/patterns-loading-intro@2x.png" width="740"/>
</div>

<br>

## Best practices

**가능한 빨리 콘텐츠를 표시하세요.**

로딩이 완료될 때까지 기다리게 하면 사용자는 콘텐츠가 없다는 것으로 여길 수 있습니다. 대신, 아직 콘텐츠가 없는 곳에는 placeholder, 그래픽, 애니메이션을 표시하고 콘텐츠가 로드되면 대체하세요. 그리고 가능하면 백그라운드에서 미리 필요한 콘텐츠를 로드하세요.

<br />

**콘텐츠가 로드되고 있다는 사실과 얼마나 걸릴지에 대한 정보를 명확하게 전달하세요.**

콘텐츠가 즉시 표시되는게 제일 좋지만 로딩이 잠시 걸리는 경우에는 시스템에서 제공하는 컴포넌트인 Progress indicator를 사용해서 콘텐츠가 로드되고 있다는 것을 표시할 수 있습니다. 일반적으로 언제까지 로딩이 소요될지 알 수 있는 경우에는 Determinate progress indicator를 사용하고, 로딩 지속시간을 측정할 수 없는 경우에는 Indeterminate progress indicator를 사용합니다.(예: macOS의 Finder는 파일 복사가 완료되기 까지 얼마나 걸릴지를 판단하는 데 도움이 되도록 Determinate progress bar와 간단한 설명 텍스트를 사용합니다) 
자세한 내용은 [Progress indicators](./progress-indicators.md)를 참고하세요.

<br />

**불가피하게 로딩이 오래 걸리는 경우 사용자가 기다리는 동안 볼 수 있는 콘텐츠를 제공하는 것도 고려해보세요.**

예를 들어 게임 플레이에 대한 힌트를 제공한다거나 짧은 비디오나 애니메이션을 재생하거나 유용한 placeholder, 그래픽을 표시할 수 있습니다. 가능하면 남은 로딩 시간을 정확하게 측정해서 대체 콘텐츠를 즐기기까지 시간을 너무 적게 주거나 반복해야 하는 시간이 너무 길지 않도록 해야 합니다.

<br />

**커스텀 로딩 뷰를 고려해보세요.**

표준 Progress indicator는 보통 사용하는데 문제가 없지만 때때로 컨텍스트에 벗어난 느낌을 줄 수 있습니다. 앱이나 게임의 스타일과 일치하는 커스텀 애니메이션 및 컴포넌트를 사용해서 더 매력적인 사용자 경험을 설계하는 것도 고려해보세요.

## Platform considerations

_iOS, iPadOS, macOS, tvOS, visionOS에 대한 추가 고려 사항은 없습니다._

### watchOS

**watchOS에서는 로딩 중에 indicator를 표시하지 마세요.**

사용자는 Apple Watch에서 빠른 상호 작용을 기대하므로 콘텐츠를 즉시 표시하는 것을 목표로 하세요. 만약에 콘텐츠가 로드되는데 1~2초 정도 걸리는 상황에서는 빈 화면보다는 indicator를 표시하는 것이 좋습니다.

## Resources

### Related

- [Launching](./launching.md)

- [Progress indicators](./progress-indicators.md)
