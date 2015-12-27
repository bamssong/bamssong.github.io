---
layout: post
title: Mac에서 Ruby 환경 준비하기
categories: []
tags: []
published: True

---

Homebrew 설치 및 rbenv를 통한 관리


Mac에서 Ruby 개발 환경 준비하기 [보러가기](https://zunonia.wordpress.com/2014/03/19/mac%EC%97%90%EC%84%9C-ruby-%EA%B0%9C%EB%B0%9C-%ED%99%98%EA%B2%BD-%EC%A4%80%EB%B9%84%ED%95%98%EA%B8%B0/)


## ruby 버젼 확인하기

```bash
$ ruby -v
ruby 2.0.0p481 (2014-05-08 revision 45883) [universal.x86_64-darwin14]
```

## Homebrew 설치하기
Mac 패키지 관리자 homebrew

```bash
$ ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

## rbenv 설치하기!! Homebrew on Mac
환경 관리 솔루션의 중 하나 rbenv가 필요한 이유는 버젼호환성을 편하게 하기 위함
[https://github.com/rbenv/rbenv](https://github.com/rbenv/rbenv)

```bash
$ brew udpate
$ brew install rbenv ruby-build
```

## rbenv 환경 설정 추가하기
install이 끝나면 아래에 출력 문구들이 나오는데 추가한다.<br>
(bash 이면, ".bashrc", zsh이면 ".zshrc" 에 추가해 준다.)

```bash
To enable shims and autocompletion add to your profile:
if which rbenv > /dev/null; then eval "$(rbenv init -)"; fi
```

설치확인

```bash
$ rbenv
rbenv 0.4.0
Usage: rbenv <command> [<args>]
...//생략
```

## 원하는 Ruby 버젼 설치하기
1.9.3 버젼 Ruby 설치하기

```bash
$ rbenv install -l
...//설치 가능 목록..

$ rbenv install 1.9.3-p545

//설치 후 해시테이블 갱신을 한다.
$ rbenv rehash
```

## 원하는 Ruby 버젼 사용하기
'rbenv global'로 변경

```bash
$ rbenv global 1.9.3.-p545 
//or 
$ rbenv global system

//확인
$ ruby -v 

$ rbenv versions
```












