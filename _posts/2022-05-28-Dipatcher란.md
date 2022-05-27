---
layout: post
title:  "Dispatcher란"
date:   2022-05-27 12:21:00 +0900
categories: jekyll update
---

코루틴에서 Dispatcher란 용어가 자주 등장하고 그 역활에 대해서 언급이 되나,
정확한 개념을 알지 못했다.

- 프로세스 관점에서 바라보기.

운영체제는 프로세스들의 실행 사이에 프로세스를 교체하고 재시작할 때 오류가 발생하지 않도록 관리해야합니다. 이를 위해 운영체제는 프로세스의 상태를 실행(running), 준비(ready), 블록(block) 상태로 분류하고 프로세스들을 상태전이(state transition)를 통해 체계적으로 관리합니다.

![프로세스상태전이](https://t1.daumcdn.net/cfile/tistory/27733D4856EEACF616)

사용자가 프로그램을 실행하면 프로세스가 생성되고 준비리스트에 추가됩니다. 프로세스는 프로세서(CPU)가 사용가능한 상태가 되면 CPU를 할당받습니다. 이를 준비상태에서 실행상태로 상태전이(state transition)된다고 합니다. 이 과정을 디스패칭(dispatching)이라고 하고 디스패처(dispatcher)가 이 일을 수행

출처: https://bowbowbow.tistory.com/16 [멍멍멍:티스토리]