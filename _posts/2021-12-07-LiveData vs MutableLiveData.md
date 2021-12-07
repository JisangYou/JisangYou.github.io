---
layout: post
title:  "LiveData vs MutableLiveData"
date:   2021-12-07 23:50:10 +0900
categories: jekyll update
---

정리중..

MutableLiveData 와 LiveData ?
MutableLiveData는 ViewModel 안에서 해당 데이터가 수정 될 수 있습니다.
LiveData는 읽을 수 있지만, 변경 되지 않습니다.
LiveData는 ViewModel 외부에서 데이터를 읽을 수 있으나, 수정되지 않게 하려면 LiveData를 통해 외부에 해당 데이터를 제공 해야 합니다.
이러한 이유는 외부에서 Livedata를 변경하지 못하게 하고, 내부에서는 변경이 가능하게 하기 위한 구현이 목적입니다.
이것은 "캡슐화"와 같은 방법입니다. 오브젝트의 필드 중 일부에 대한 직접 접근을 제한하는 방법입
출처: https://yoon-dailylife.tistory.com/45 [알면 쓸모있는 개발 지식]