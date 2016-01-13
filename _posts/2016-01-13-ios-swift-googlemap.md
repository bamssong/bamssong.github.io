---
layout: post
title: iOS swift 구글맵 이용하기
categories: []
tags: []
published: True

---

iOS swift, Google Maps SDK이용한 간단한 설명글

[Google Maps SDK for iOS](https://developers.google.com/maps/documentation/ios-sdk/)<br>
[Google Places API for iOS](https://developers.google.com/places/ios-api/)<br>

위 링크에 가면 자세한 설명과 편하게 가져다가 쓸 수 있는 샘플 코드도 제공하기 때문에 간단하게
중요한 포인트만 정리



## 들어가기전
Xcode 6.3이상, [CocoaPods](/ios-cocoapod-start)를 사용

cocoapod 설정

```
source 'https://github.com/CocoaPods/Specs.git'
platform :ios, '8.1'
pod 'GoogleMaps'
```

## API key 발급 (구글 계정 필요)
[Google Developers Console](https://console.developers.google.com/flows/enableapi?apiid=maps_ios_backend&keyType=CLIENT_SIDE_IOS&reusekey=true)


## [밤쏭이 만들 샘플 코드 보기](https://github.com/bamssong/ios-swift-sample/tree/master/cocoapod/GoogleMap)
- google map을 UIView로 연결처리
- marker 관련 처리
- camera 업데이트 처리
- place Autocomplete 연결 처리
