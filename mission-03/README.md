# Mission-03

- 소개
- 결과
- Markup 구조
</br>

## 소개
web cafe 시안 중 관련 사이트 부분을 구현한 결과입니다.
</br>
</br>

## 결과

![transition_result](https://github.com/chowonn/home-work/assets/70478015/11a8362c-74f9-4a02-9448-0b7a0510ad3f)


## Markup 구조
```
body
└── section.site-container
    ├── h2.head 
    └── div.site-contents
         └── ul.dropdown
           ├── li
           │   └── a 
           ├── li.drop_list
           │   └── a 
           ├── li.drop_list
           │   └── a
           ├── li.drop_list
           │   └── a 
           └── li.drop_list
               └── a
   
```
- 전체 section으로 묶어준 후 dropdown 될 영역을 잡아주고 각각의 li를 클릭했을 때 해당 사이트로 이동하도록 하이퍼링크를 주었습니다.
- .site-contents 영역에 hover되기 전 1개의 목록만 보일 수 있도록 영역 밖은 overflow: hidden 으로 텍스트를 숨겼습니다.
- hover 되었을 때 드롭다운되는 부분은 .site-contents 이 먼저 내려오고 리스트들은 시간차를 두고 내려오는데, 이는 .site-contents:hover height와 .site-contents:hover ul의 padding-top 부분에 transition duration과 delay 속성으로 해결했습니다.

