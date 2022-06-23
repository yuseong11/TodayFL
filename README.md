# TodayFL

### “오늘 전장” 게임 일정을 알려주는 크롬 확장 프로그램

**개인 프로젝트 | 2022.03 (일주일)**

![image](https://user-images.githubusercontent.com/82145837/174545743-bea64eda-fa0d-44a1-9841-89c0ea326aef.png)

### 개요

게임하며 4년간 겪은 불편함을 해결하기 위해 만든 크롬 확장 프로그램입니다. 게임에서 총 4개의 맵이 매일 0시 주기로 바뀝니다. 이 순서를 게임에 접속하지 않고 확인하기 위해 제작했습니다.

### 사용기술

`Javascript` `Tailwind`

### 고민했던 문제와 해결과정

> 왜 이전에 만든 비슷한 기능의 사이트는 인기가 없지? 어떻게 하면 사용자가 늘어날까.

- 접근성, 사용성, UIUX 디자인 등 복합적인 문제 ([자세한 내용](https://www.notion.so/1797afad5fc043bda8ab72cc908c0cce))\*\*

  사실 2021년 10월에 비슷한 목적으로 웹사이트를 제작했습니다. 개인적으로는 만족한 프로젝트였으나 실방문자가 하루에 적었습니다. 제가 생각해봤을 때 문제점은 크게 세 가지였고 해결방안은 두가지였습니다.

  **문제점 1. 접근성이 부족하다.**

  이 사이트는 구글에 검색해도 나오지 않는다. 그때는 SEO 설정하고 구글 서치 콘솔만 적용하면 사이트가 등록되는 줄 알았다. sitemap.xml 이나 robot.txt은 몰랐다. 링크를 타고 들어온 사람은 게임 커뮤니티 사이트에 홍보된 글을 타고 들어왔다. 당연히 신규 접속자가 적을 수 밖에 없었다.

  **문제점 2. 처음 사이트에 들어왔을 때 오늘 전장이 무엇인지 정확히 보이지 않는다.**

  오늘 전장이라는 이름이 무색할 정도다. 오늘 날짜는 달력 배경색이 변하도록 했는데 파스텔톤이라서 눈에 띄지 않는다. 또 이름을 표시한 상자도 색이 알록달록해서 통일성이 없고 텍스트와 대비가 확실하지 않다.

  **문제점 3. 사용성이 떨어진다.**

  검색 되지 않기때문에 사용자가 사이트를 즐겨찾기 추가하거나 URL을 외워야한다. 두 방법 모두 번거롭기 때문에 선뜻하지 않을 것 같았다.

  **해결 방법 1. 접근성 해결: 크롬 확장 프로그램으로 등록하기**

  SEO를 위해 따로 처리하지 않아도 검색 엔진에 등록되고, 매번 사이트에 접속하지 않으니 사용성도 훨씬 좋아진다.

  **해결 방법 2. UI 수정: 한달 전장 일정이 아니라 오늘 전장만 나오도록 하기**

  한달 달력이 모두 나오면 UI적으로 복잡해질 수 밖에 없다. 다른 요소는 제외하고 오늘의 전장이 무엇인지만 나타내면 확장 프로그램적으로도 어울리고 유저 입장에서 더 편할 거라 예상했다.

  이런 방법을 적용해본 결과 과거 10명에 못 미치던 사용자에서 현재는 350명(220726)로 증가했습니다.

> 4일마다 반복되는 로직을 날짜함수로 어떻게 짜야할까?

- 날짜 사이의 기간을 구해서 주기별로 나누는 로직

### 관련 포스팅

- [크롬 확장프로그램 제작 후기](https://www.notion.so/1797afad5fc043bda8ab72cc908c0cce)
- JavaScript에 내장된 [Date 메서드와 관련 라이브러리 사용법](https://www.notion.so/2a225222cf184cbeb72669210d9c38c1)
- [tailwind 라이브러리](https://www.notion.so/Tailwind-CSS-48b2007271e44746a2b881286375d28f) CLI 설치, 빌드 방법
