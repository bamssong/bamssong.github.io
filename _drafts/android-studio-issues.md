---
layout: post
title: Android Studio 이슈 모음
categories: []
tags: []
published: True

---

안드로이드 스튜디오를 사용하면서 발생되는 문제들을 모아둔 공간

## taskArtifacts/cache.properties 파일이 없다는 이슈

```
.gradle/2.8/taskArtifacts/cache.properties
```

해결 >>

```
rm -rf /Users/Abhishek/muftbytes-androidapp/.gradle
//try clean build
```