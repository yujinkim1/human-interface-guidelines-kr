---
create-date: 2023-12-15
update-date: 2023-01-12
supported-platforms: iOS, iPadOS, macOS, tvOS, visionOS, watchOS
---

# Loading

<h2>콘텐츠가 로드되는 동안 빈 화면이나 정적인 콘텐츠를 표시하지 마세요. 이러면 사용자는 앱이나 게임이 느려지거나 멈춘 것으로 인지할 수 있습니다.</h2>

<div align="center">
  <img alt="patterns-loading-intro" src=".attachments/.loading/patterns-loading-intro@2x.png" width="740"/>
</div>

## Best practices

**가능한 빠르게 콘텐츠를 표시할 수 있도록 하세요.**

로딩이 완료되기를 기다리게 만들면 사용자는 콘텐츠가 없다는 것으로 여길 수 있습니다. 대신, 아직 콘텐츠가 없는 곳에는 placeholder 텍스트, 그래픽, 애니메이션을 표시하고 콘텐츠가 로드되면 대체될 수 있도록 하세요. 그리고 가능한 경우 필요한 콘텐츠를 미리 로드하세요.(예: 애니메이션이 재생되거나 사용자가 메뉴를 탐색하는 동안)

<br />

**콘텐츠가 로드되고 있다는 사실과 얼마나 걸릴지에 대한 정보를 명확하게 전달하세요.**

콘텐츠가 즉시 표시되는게 이상적이지만 로딩이 잠시 걸리는 경우에는 시스템에서 제공하는 컴포넌트인 progress indicator를 사용해서 콘텐츠가 로드되고 있다는 것을 표시할 수 있습니다. 일반적으로 언제까지 로딩이 소요될지 알 수 있는 경우에는 determinate progress indicator를 사용하고, 로딩 지속시간을 측정할 수 없는 경우에는 indeterminate progress indicator를 사용합니다.(예: macOS의 Finder는 파일 복사가 완료되기 까지 얼마나 걸릴지를 판단하는 데 도움이 되도록 determinate progress bar와 간단한 설명 텍스트를 사용합니다.) 자세한 내용은 [Progress indicators](./progress-indicators.md)를 참고하세요.

<br />

**불가피하게 로딩이 오래 걸리는 경우 사용자가 기다리는 동안 볼 수 있는 콘텐츠를 제공하는 것을 고려해보세요.**

예를 들어 게임 플레이에 대한 힌트를 제공한다거나 짧은 비디오나 애니메이션을 재생하거나 유용한 placeholder 그래픽을 표시할 수 있습니다. 가능하면 남은 로딩 시간을 정확하게 측정해서 콘텐츠를 즐기기까지 너무 적은 시간을 제공하거나 반복해서 보여주는 상황을 피해야합니다.

<br />

**커스텀 로딩 뷰를 고려해보세요.**

표준 progress indicator는 보통 사용하는데 문제가 없지만 때때로 컨텍스트에 벗어난 느낌을 줄 수 있습니다. 앱이나 게임의 스타일과 일치하는 커스텀 애니메이션 및 컴포넌트를 사용해서 더 매력적인 사용자 경험을 설계하는 것을 고려하세요.

## Platform considerations

*iOS, iPadOS, macOS, tvOS, visionOS에 대한 추가 고려 사항은 없습니다.*

### watchOS

**watchOS에서는 로딩 중에 indicator를 표시하는 것을 피하세요.**

사용자는 Apple Watch에서 빠른 상호 작용을 기대하므로 콘텐츠를 즉시 표시하도록 노력해야 합니다. 콘텐츠가 로드되는데 1~2초 정도 걸리는 상황에서는 빈 화면보다는 indicator를 표시하는 것이 좋습니다.

## Resources

### Related

[Launching](./launching.md)

[Progress indicators](./progress-indicators.md)
