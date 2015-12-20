---
layout: post
title: iOS COCOAPOD 사용하기
categories: []
tags: []
published: True

---

[COCOAPOD](https://cocoapods.org/)란? Swfit & Object-C iOS 라이브러리 의존성 관리 도구.

## 설치하기

``` bash
$ sudo gem install cocoapods
```

## 시작하기

- xcode로 생성한 프로젝트 폴더 경로에서 Podfile을 생성.

```bash
//(path in xxx.xcodeproj)
$ pod init
```

- 아래와 같이 필요한 lib를 pod 'XXX'로 추가하면된다.

```text
platform :ios, '8.0'
use_frameworks!

target 'MyApp' do
  pod 'AFNetworking', '~> 2.6'
  pod 'ORStackView', '~> 3.0'
  pod 'SwiftyJSON', '~> 2.3'
end
```

예 [alamo fire](https://github.com/Alamofire/Alamofire) : network lib

```text
source 'https://github.com/CocoaPods/Specs.git'
platform :ios, '8.0'
use_frameworks!

target 'MyApp' do
  pod 'Alamofire', '~> 3.0'
end
```

- 인스톨 

```bash
pod install
```

- 실행하기
xxx.xcodeproj가 아닌 xxx.xcworkspace로 실행해야한다.

```bash
$ xxx.xcworkspace
```
