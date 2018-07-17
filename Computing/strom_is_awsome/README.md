# 히어로즈 오브 더 스톰 : 시공의 폭풍

![hios preview](https://cdn.frontend.moe/photos/hios.gif)

2016-2017년 사이에서 "히어로즈 오브 더 스톰" 온라잉ㄴ 게임이 인터넷 상의 패러디의 대상으로 유행이 돈 적이 있음.

여러 작품 중에 '히어로즈 오브 더 스톰' 게임 심볼을 소용돌이 삼아  CSS의 `transform` 기능으로 모든 HTML 요소가 빨려드려가는 애니매이션을 보여주는 작품이 기억남.
> [도탁스 (DOTAX) | 🌀🌀🌀🌀🌀🌀 히어로즈 오브 더 탁스 🌀🌀🌀🌀🌀🌀](http://cafe.daum.net/dotax/FGFP/9109?q=%C8%F7%BE%EE%B7%CE%C1%EE%20%BF%C0%BA%EA%20%B4%F5%20%C5%B9%BD%BA%20%EC%8B%9C%EA%B3%B5%EC%9D%98%20%ED%8F%AD%ED%92%8D%EC%9D%80%20%EC%A0%95%EB%A7%90%20%EC%B5%9C%EA%B3%A0%EC%95%BC)

개인적으로 '회전'이라 하면 가장 먼저 생각나는 작품이라, [해당 작품을 프로세싱으로 구현해봤습니다.](./strom-is-awsome.pde)

## 사용된 Transform 관련 메서드

`rotate(), scale(), translate()`

## `processing.sound.*` 라이브러리 설치

애니매이션과 함께 `hios_is_awsome.mp3`, `i_love_hios_x3.mp3` 을 재생하기 위해 외부 모듈이 필요합니다.

`Sketch -> import Library -> Add Library -> Sound` 설치