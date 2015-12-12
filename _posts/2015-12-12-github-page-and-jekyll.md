---
layout: post
title: Github Page & Jekyll
---
jekyll로 블로그 시작하기


*! MAC 사용자 기준으로 작성 했습니다.*


## Jekyll 준비하기 
> 자세한 설명? [http://jekyllrb.com/](http://jekyllrb.com/)<br>
> 번역 : [http://jekyllrb-ko.github.io/](http://jekyllrb-ko.github.io/)

1. **설치**<br>

	```
	$ gem install jekyll
	$ jekyll new my-awesome-site
	$ cd my-awesome-site
	$ ~/my-awesome-site jekyll serve
	```
2. **서비스 돌려보기**<br>

	```
	웹 브라우져 서비스 시작  : http://localhost:4000 에 접속
	서비스 종료 : control + c
	```
	**gem?** 'apt-get'와 비슷한 분산 패키지 시스템

## Github Page에 올리기
> 자세한 설명? [https://pages.github.com/](https://pages.github.com/)



1. **github repository 만들기**<br>
	name : you_name.github.io 으로 하고 생성한다.

2. **github repository에 Jekyll 올리기** <br>
	생성 후 github에 해당 저장소 설명을 보면  git 설정하는 부분이 나온다.

	```
	$ echo "# bamssong.github.io" >> README.md
	$ git init
	$ git add README.md
	$ git commit -m "first commit"
	$ git remote add origin https://github.com/bamssong/bamssong.github.io.git
	$ git push -u origin master
	```


	'git push' 하면 username / password를 물어보는데, github 계정 id/pw 을 적으면된다.

3. **확인하기**
	
	```
	웹 브라우져 확인 : http://bamssong.github.io
	```






