## 개요
- jekyll 기반으로 호스팅되므로 jekyll 의 기본 프로젝트 구조 및 의미는 [다음](https://jekyllrb-ko.github.io/docs/structure/) 을 참고하세요.  

## 게시물 작성
- 작성되어 게시될 포스트들은 `_post` 디렉토리 하위의 `YEAR-MONTH-DAY-title.md` 와 같은 형식으로 저장되어야 합니다.   
    ```
    2022-12-27-sonarkube-java-spring8-try-with-resources.md   
    2023-01-01-new-year-에도-코딩을-하다니.md
    ```
- 게시글의 처음은 [front-matter](https://jekyllrb-ko.github.io/docs/front-matter/) 형식으로 작성되어야 합니다. 간단하게 아래와 같은 양식으로 작성될 수 있습니다.
    ```
    ---
    layout: post
    title:  "java8 try-with-resources compliant code example."
    ---
    
    # java8 에 도입된 try-with-resources 는 아래와 같이 사용될 수 있습니다.
    
    ### Compliant Code
    ...
    ```
- Rules 번역 시, 카테고리화를 위해 아래의 박스친 항목들을 태그화 혹은 카테고리화 하여 관리해야 합니다.  
  ![guide-image](./document/images/transliate-guide.png)  
태그는 front-matter 항목에 tags 혹은 categories 에 배열 형식으로 작성할 수 있습니다.  
  ```
  2022-12-28-collect-with-streams-instead-of-list::add.md
  ---
  layout: post
  title:  "collect 는 thread-safe 합니다."
  (tags || categories): [java8, Minor]
  ---
  ```
- 아직 포스트 작성이 완료되지 않거나, 발행을 원치 않는 포스트들은 `_drafts` 하위 폴더에 md 파일을 작성해주세요.
  ```
  .
  ├── _drafts
  │   └── 아직-미완성한-파일이에요.md
  ...
  ```