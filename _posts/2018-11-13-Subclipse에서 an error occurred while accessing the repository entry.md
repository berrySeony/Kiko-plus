---
layout: post
title: "Subclipse에서 an error occurred while accessing the repository entry"
description: "SVN connection refuse"
date: 2018-11-13
comments: true
---

오랜만에 이클립스를 사용하게 되었는데, 오류는 심플하다. 갑자기 SVN / CVS 가 연결이 되지 않는다. 
그동안 아무런 문제없이 써왔던 SVN이 아무 설정도 건들이지 않았는데도 CONNECT REFUSE 알람이 뜬다. 
'an error occurred while accessing the repository entry' 와 같은..
개인적인 생각으로는 SVN서버가 재구성이 되어서 설정을 다시 잡아줘야 하는 문제 같다. 

1. http://june2008b.blogspot.com/2014/08/usernamepassword-subclipse.html
결론으론 난 이걸론 해결을 되지 않았다

그래서 subclipse가 갑자기 업데이트가 되어서 안되었나 생각해서, 이클립스 업데이트를 선택하게 되었다
그런데 이것도 안된다 이때부터 이클립스 자체의 네트워크 커넥션 문제인 것을 알게되었다

2. https://stackoverflow.com/questions/41720780/cannot-open-eclipse-marketplace-cannot-install-remote-marketplace-locations-can
이것으로 해결
subclipse가 안되면 거진 서버 자체의 문제인경우가 많은데, tortoise 를 설치해서 테스트 해보니까 잘 되어서 이클립스 자체의 문제인건 알았지만,
대체 이런 오류가 생긴 이유를 모르겠다.
