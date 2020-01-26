---
path: 'react01'
date: '2020-01-26 16:33:56'
title: '무작정 따라 하는 리액트 - 이벤트'
---

> **이 강좌는 지식을 얻는 것보다 무작정 따라 하며 코딩에 익숙해지는 것이 목적입니다.** 더 쉬운 설명을 위해 잘못된 설명이 있을 수 있습니다. 무작정 따라 하며 익숙해진 뒤 잘못된 부분들을 찾아보세요.

## 목차

1. [이벤트란](#이벤트란)
2. [이벤트 종류](#이벤트-종류)
3. [이벤트 처리](#이벤트-처리)

## 이벤트란

이벤트는 웹과 사용자가 상호작용하기 위한 도구입니다. 사용자가 어떤 행위를 했을 때 웹이 그에 맞는 작업을 수행하기 위해서 미리 작성해 두는 것입니다. 즉 순서대로 실행되는 것이 아니라 어떠한 행위(이벤트)가 발생했을 때 실행될 작업을 미리 작성해두는 것입니다.

## 이벤트 종류

이벤트는 사용자의 행위를 기다렸다가 수행하는 것이기 때문에 어떤 행위인지를 정해서 기다려야합니다. 몇가지 자주 사용하는 이벤트들이 있습니다.

| 리스너 메소드 | 이벤트                                                   |
| ------------- | -------------------------------------------------------- |
| onClick       | 해당 엘리먼트를 클릭했을 때 발생                         |
| onChange      | 입력을 처리하는 form 인 경우에 입력이 변경되었을 때 발생 |
| onKeyDown     | 키보드가 눌렸을 때 발생                                  |
| onMouseOver   | 해당 엘리먼트 위에 마우스가 올라왔을 때 발생             |
| onMouseOut    | 해당 엘리먼트 위에 있던 마우스가 벗어났을 때 발생        |

## 이벤트 처리

이벤트를 처리하기 위해서는 특정 엘리먼트에게 1)`어떠한 이벤트가 발생했을 때` 2)`어떤 작업을 처리`하도록 해주어야합니다.

`어떤 이벤트가 발생했을 때`를 감지하기 위해서 해당 엘리먼트가 그 이벤트를 기다려야 합니다. 이것을 `listening`한다고 표현하는데 이벤트를 `listen`하는 역할을 하는 것이 **이벤트 리스너**입니다. 각 이벤트 종류마다 리스너가 존재하기 때문에 어떤 리스너를 호출할 지 선택해야합니다.

이제 해당 리스너에게 `어떤 작업을 처리`하도록 시켜야 하는데 이를 쉽게 **이벤트 핸들러**라고 표현합니다. 이 것은 어떠한 작업이기 때문에 반드시 **함수**여야합니다.

즉, 특정 엘리먼트에 원하는 이벤트 리스너에게 이벤트 핸들러를 전달하면 해당 이벤트가 발생했을 때 이벤트 핸들러에 작성된 함수가 실행되는 것입니다.

다음장에서 직접 실습해보도록 하겠습니다.