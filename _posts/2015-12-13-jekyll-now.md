---
layout: post
title: Jekyll Now 사용하기
---

특별한 개발지식이 없더라도 쉽고 가볍게 'Jekyll Now'를 이용해서 Github Page 만들기

참고 : 일몰 블로그 [Jekyll,Git 을 몰라도 무료 Github Pages 즐기기](http://ilmol.com/2015/01/Jekyll,Git%20%EC%9D%84%20%EB%AA%B0%EB%9D%BC%EB%8F%84%20%EB%AC%B4%EB%A3%8C%20Github%20Pages%20%EC%A6%90%EA%B8%B0%EA%B8%B0.html)<br>
Jekyll Now [바로가기](http://www.jekyllnow.com/)


## 순서
1. github 가입
2. jekyll-now 사용
3. 글 올리기
4. 글 확인하기
5. About 수정하기

tip 1. 작업 중인 포스트 공간? '_drafts'<br>
tip 2. 로컬에서도 확인? 

----
## 1. github 가입
- [github](https://github.com/)가서 회원 가입


## 2. jekyll-now 사용
- [jekyll-now 이동](https://github.com/barryclark/jekyll-now)<br>
- 화면 우측상단에 ![fork]({{ site.baseurl }}/images/jekyll-now-fork.png) 을 선택 <br>
- fork 후 설정에 'Repository name' 수정 'github_id.github.io'<br>
- '_config.yml' 파일을 열어서 필요한 정보를 넣어준다.

```
name: bamssong
description: UX/UI & Android/iOS & Ruby?
avatar: https://s.gravatar.com/avatar/d665410aea0cdd6aa0ad1f31714daed7?s=80
```


## 3. 글 올리기

![jekyll-post]({{ site.baseurl }}/images/jekyll-post.png "jekyll post 하기")

- 우측상단에 'New file'선택 후 'YYYY-MM-DD-title.md' 형식으로 파일을 생성

```
---
layout: post
title: Jekyll Now 사용하기
---
마크다운 형식에 블로그 내용
```
- 글 작성 후 'Commit new file'에 작업 기록을 남기고 (안남겨도 된다) 'Commit new file' 버튼을 선택한다.


## 4. 글 확인하기

- **http://bamssong.github.io** 이동해서 확인.

## 5. About 수정하기
/about.md 파일을 수정하면 됩니다.

![jekyll-about]({{ site.baseurl }}/images/jekyll-now-about.png "jekyll now about 수정하기")



## tip 1. 작업 중인 포스트 공간? '_drafts'

- 아직 공개하고 싶지 않은 글이 있는경우 _drafts 폴더를 만들어서 '3. 글 올리기' 작업을 하면 된다.


## tip 2. 로컬에서도 확인?
- 로컬에서 작업하고, 로컬 서버를 통해서 확인 후 리모트 저장소에 올리고 싶을 때 사용하면 된다.

```
1. Install Jekyll and plug-ins in one fell swoop. 
gem install github-pages This mirrors the plug-ins used 
by GitHub Pages on your local machine including Jekyll, Sass, etc.

2. Clone down your fork git clone git@github.com:yourusername/yourusername.github.io.git

3. Serve the site and watch for markup/sass changes jekyll serve

4. View your website at http://127.0.0.1:4000/

5. Commit any changes and push everything 
to the master branch of your GitHub user repository. 
GitHub Pages will then rebuild and serve your website.
```

