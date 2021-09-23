---
layout: post
title:  "git clone이 되지 않음 (clone into... 에서 hang)"
date:   2021-09-19 23:57:27 +0900
categories: git
---
방화벽 문제 확인

1. 제어판 → 프로그램 → windows 기능 켜기/끄기 →  텔넷 클라이언트 체크
2. `CMD` → TELNET [github.com](http://github.com) 80 (github.com 에 80 port로 접근가능한지)
3. 정상적으로 통신됨 → 방화벽 문제X

`gitbash`가 아닌 윈도우 `CMD`로 git clone

1. 해당폴더 접근 → git clone
2. 정상 해결

참고 : [www.lainyzine.com] 

[www.lainyzine.com]:  [https://www.lainyzine.com/ko/article/git-clone-command/#https-프로토콜로-git-저장소-clone](https://www.lainyzine.com/ko/article/git-clone-command/#https-%ED%94%84%EB%A1%9C%ED%86%A0%EC%BD%9C%EB%A1%9C-git-%EC%A0%80%EC%9E%A5%EC%86%8C-clone)
