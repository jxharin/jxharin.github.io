---
title:  "Node.js npm aduit?!"
excerpt: "리액트 사용 중 발생한 npm 에러"

categories:
  - nodejs
tags:
  - [React, Node.js, JavaScript, npm, aduit]

toc: true
toc_sticky: true
 
date: 2024-01-22
last_modified_at: 2024-01-22
---

## npm aduit?!
![ex_screenshot](/assets/img/npmerror.png)


React 강의를 들으며 실습하던 와중, npm install styled-componenets를 install 하면서 이런 오류가 발생하였다

npm aduit? NSP의 데이터베이스를 이용해서 취약점을 점검해 주는 기능!
npm fund? pm fund는 내 프로젝트에서 사용하고 있는 package들을 만들고 관리하는 회사들에게 후원할 수 있는 사이트 목록을 출력해주는 명령어!

딱히 에러를 나타내진 않다고 하지만 에러메세지처럼 붉은 글씨들과 못 알아듣겠는 와다다다... 
해결하여 말끔하게 install하고 싶어서 알아봤다!

aduit은 각 패키지들이 가진 취약점을 체크해주는 로직이 들어 왔다는 뜻으로, 
npm 패키지 자체가 install 시에 물고물고물린 의존성에 따라 여러 패키지들을 알아서 설치해주다보니, 그 과정에 발생할 수 있는 이슈를 대비하기위해 해주는 거라고 한다.

출처: https://blinders.tistory.com/75 [글쓰는 개발자:티스토리]

```
npm set aduit false
```
를 통해 aduit 기능을 끄고, --no-fund를 붙여 install 하자!

![ex_screenshot](/assets/img/npminstall.png)

말끔하게 설치 완료!✌️