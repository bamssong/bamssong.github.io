---
layout: post
title: iOS 기기별 해상도와 좌표
categories: []
tags: []
published: True

---

iOS 기기에 따른 해상도관련 정리.

추천 : 샤코님의 글 [iOS 8의 적응형(Adaptive) UI](http://www.shako.net/blog/ios8-adaptive-ui-explained/)


## 사이즈 클래스 (Size classes)
**Regular** : 큰 크기<br>
**Compact** : 작은 크기<br>

## 기기의 방향과 크기별 사이즈 클래스 (W-H)

**아이패드** : Regular - Regular (가로,세로)<br>
**5.5인치(아이폰6+)** : Compact - Regular (세로), Regular - Compact (가로)<br>
**4인치(아이폰 5.6)** : Compact - Regular (세로), Compact - Compact (가로)<br>

## 트레잇 컬렉션(Trait Collection)
현재 스크린 정보를 담고 있는 곳

horizontalSizeClass : compact, regular<br>
verticalSizeClass : compact, regular<br>
interface Idium : 아이폰 또는 아이패드 구분<br>
displayScale : 화면 비율 정보<br>
