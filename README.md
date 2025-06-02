# 프로젝트 소개
#### 💻 프로젝트명
  대관령 음악제

#### 🛠 사용한 기술
  HTML, SCSSS, JQUERY

#### 🎯 모작 이유
  마우스 커서 제어, 헤더 스타일 변경 등 다양한 jQuery 기능을 직접 구현해보고 싶었고, SCSS를 활용해 구조적인 코드 작성을 연습해보고 싶어서 이 사이트를 모작하게 되었습니다.

#### 😱 어려웠던 점
 - 하나의 이벤트 리스터 안에 여러 기능을 동시에 제어하는 것이 어려웠습니다.
 - grid-template 속성을 사용하여 여러 아이템을 일정한 비율로 배치하는 것이 생각보다 까다로웠습니다.
 - scss를 이용하니 반응형 코드 작성시 각 섹션마다 일일이 입력하고, 선택자를 찾는 것이 번거로웠습니다.

---
# 🔍 self code preivew

### 📁 파일 구조 및 구성
- [ ] 역할별로 디렉토리 분리 (/css, /js, /images) <br>
  -> js파일 분리 못함...
- [x] 파일/폴더 네이밍 일관성 유지
- [ ] 공통 요소(헤더, 푸터 등) 분리하여 재사용 구조 설계 <br>
  ->메인페이지만 모작하느라 분리 못함...
- [x] 파일 구조가 한눈에 파악되도록 정리됨
- [x] 필요 없는 파일/코드 제거하여 깔끔하게 마무리
- [x] 이미지 파일 사이즈 최적화 및 이름 명확하게 지정
- [x] HTML 파일은 의미 있는 이름으로 저장 (ex. `index.html`, `about.html` 등)

---

### ⌨ HTML 리뷰
```html
      <footer class="footer">
        <div class="inner">
            <div class="item_01">
                <p class="title">(재)강원문화재단 대관령음악제운영실</p>
```
#### 1.시맨틱(semantic) 마크업
- [x] header, main, footer, section, article 등 시맨틱 태그를 적절히 사용했는가?
- [ ] div와 span을 남용하지 않았는가?
- [ ] 문서 구조가 논리적으로 잘 구성되어 있는가?

#### 2. 구조 및 계층
- [x] 들여쓰기가 일관적으로 되어 있는가?
- [x] 중첩 구조가 너무 깊거나 복잡하지 않은가?
- [x] 불필요한 태그가 없는가?

#### 3. 접근성
- [x] alt 속성이 모든 이미지에 포함되어 있는가?
- [x] heading 태그(h1~h6)가 순차적으로 사용되었는가?
- [x] 링크 텍스트가 명확하고, 중복되지 않는가?

#### 4. 코드 품질
- [x] ul / ol / dl 태그를 적절히 사용했는가?
- [x] button / a 태그의 역할이 명확하게 구분되어 있는가?
- [x] 텍스트 콘텐츠는 구조에 맞는 태그(p, strong, em, blockquote 등)를 사용했는가?

---

### 🎨 css 리뷰
```css
      .info_wrap {
        overflow: visible;
        cursor: none !important;

        .concertSwiper {
            overflow: visible;

            .swiper-wrapper {
                align-items: flex-end;

                .swiper-slide {
                    width: 390px;
                    transition: 1s;
                    overflow: hidden;
```
#### 1. 코드 구조 및 설계
- [x] 스타일 시트가 목적에 따라 분리되어 있는가? (reset.scss, layout.scss, component.scss 등)
- [ ] 선택자 구조가 너무 깊거나 복잡하지 않은가? (.wrap .box .title span ← 이런 거 너무 많지 않게) <br>
=> scss를 이용하다보니까 선택자 구조가 깊어지게 된듯...
- [x] 공통 스타일은 재사용 가능한 형태(.btn, .card, .title 등)로 만들어졌는가?
- [x] 불필요하게 중복된 스타일은 없는가?

#### 2. 스타일 작성 방식 
- [x] id보다는 class 위주로 스타일을 적용했는가?
- [x] 인라인 스타일 사용을 피하고 외부 스타일로 관리했는가?
- [x] !important는 꼭 필요한 경우에만 사용했는가?

#### 3. 레이아웃 & 정렬
- [x] flexbox 또는 Grid를 적절히 사용했는가?
- [x] 정렬이나 배치 속성이 의도대로 잘 작동하고 있는가? (align-items, justify-content, gap, grid-template-columns 등)
- [x] 마진/패딩이 일관성 있게 적용되었는가? (불필요한 margin-bottom, 중복된 여백 등 점검)

#### 4. 반응형 & 뷰포트 대응
- [x] 미디어 쿼리를 적절히 활용했는가?
- [x] 뷰포트 크기 변화에 따라 요소가 잘 배치되는가?
- [x] 글자 크기, 버튼 크기 등 터치 환경에서 충분한 간격이 확보되었는가?

---

### ⚙ JavaScript 리뷰
