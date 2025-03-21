# 들어가기 앞서

Markdown은 **텍스트 기반의 마크업 언어**로, 2004년 [John Gruber](https://daringfireball.net/)에 의해 만들어졌습니다.   
이 언어의 가장 큰 특징은 **간단한 문법으로 웹에서도 쉽게 문서를 작성할 수 있다는 점**입니다.

## 1. Markdown의 필요성
---
Markdown은 **HTML로 변환이 가능**하며, 특수기호와 문자를 이용한 간단한 구조를 사용합니다.     
특히 **GitHub(깃허브)** 에서 많이 사용되며, 저장소(Repository)에서 **README.md** 파일로 프로젝트 정보를 제공하는 데 활용됩니다.

> **💡 깃허브에서 README.md가 중요한 이유?**  
> - 프로젝트의 개요를 빠르게 이해할 수 있음  
> - 설치 방법, 사용법, 이슈 등을 효과적으로 전달 가능  
> - 코드 블록, 링크, 이미지 등을 활용해 가독성 향상  

---

## 2. Markdown의 기본 문법
### ✅ 제목(Header) 사용하기
프로젝트의 문서를 체계적으로 정리하기 위해 `#` 기호를 활용할 수 있습니다.

```md
# 이것은 H1 입니다.
## 이것은 H2 입니다.
### 이것은 H3 입니다.
#### 이것은 H4 입니다.
##### 이것은 H5 입니다.
###### 이것은 H6 입니다.

```
## 결과값

# 이것은 H1 입니다.
## 이것은 H2 입니다.
### 이것은 H3 입니다.
#### 이것은 H4 입니다.
##### 이것은 H5 입니다.
###### 이것은 H6 입니다.
---
### ✅ BlockQuote (인용문)
이메일에서 사용하는 > 기호를 활용하여 인용문을 작성할 수 있습니다.

```md
> 이것은 첫 번째 인용문입니다.
>	> 이것은 두 번째 인용문입니다.
>	>	> 이것은 세 번째 인용문입니다.
```

## 결과값
> 이것은 첫 번째 인용문입니다.
>	> 이것은 두 번째 인용문입니다.
>	>	> 이것은 세 번째 인용문입니다.
---

### ✅ 목록(List) 사용하기
순서 있는 목록을 만들 때는 숫자와 점(.)을 사용합니다.

### ✅ * 순서 있는 목록 (번호 목록)

```md
1. 첫번째
2. 두번째
3. 세번째
```

## 결과값
1. 첫번째
2. 두번째
3. 세번째

### ✅ * 순서 없는 목록 (글머리 기호)

```md
* 빨강
  * 녹색
    * 파랑

+ 빨강
  + 녹색
    + 파랑

- 빨강
  - 녹색
    - 파랑
```
## 결과값

* 빨강
  * 녹색
    * 파랑

+ 빨강
  + 녹색
    + 파랑

- 빨강
  - 녹색
    - 파랑

### ✅ * 혼합된 목록
```md
* 1단계
  - 2단계
    + 3단계
      + 4단계
```
## 결과값
* 1단계
  - 2단계
    + 3단계
      + 4단계

---

### ✅ 코드
Markdown에서 들여쓰기를 사용하면 코드 블록이 생성됩니다.   
4개의 공백 또는 1개의 탭을 사용하면 코드 블록으로 변환됩니다.

✅ 기본 들여쓰기 사용 예제
```md
이 영역은 일반적인 문단임

    This is a code block.
    
코드가 끝남.
```
## 결과값
이 영역은 일반적인 문단임

    This is a code block.
    
코드가 끝남.

✅ 한 줄 띄어쓰지 않으면 인식이 안되는 문제
```md
이 영역은 일반적인 문단임
    This is a code block.
코드가 끝남.
```
## 결과값
이 영역은 일반적인 문단임
    This is a code block.
코드가 끝남.

---

### ✅ 코드 블록 (Code Block)   
Markdown에서 코드블럭을 작성하는 방법은 두 가지가 있습니다.

✅ 방법 1: ```<pre><code>``` 태그 사용   
HTML의 ```<pre>와 <code>``` 태그를 사용하여 코드 블록을 만들 수 있습니다.

```md
<pre><code>
public class BootSpringBootApplication {
  public static void main(String[] args) {
    System.out.println("Hello, JB");
  }
}
</code></pre>
```

## 결과값

<pre><code>
public class BootSpringBootApplication {
  public static void main(String[] args) {
    System.out.println("Hello, JB");
  }
}
</code></pre>

✅ 방법 2: 백틱(```)을 이용

```
public class BootSpringBootApplication {
  public static void main(String[] args) {
    System.out.println("Hello, JB");
  }
}
```
---
### ✅ 수평선
Markdown에서는 수평선을 사용하여 내용을 구분할 수 있습니다.   
아래의 방법을 사용하면 수평선을 만들 수 있습니다.

```md
* * *

***

*****

- - -

---------------------------------------

```

## 결과값

* * *

***

*****

- - -

---------------------------------------

### ✅ 링크
Markdown에서 링크를 생성하는 방법은 여러 가지가 있습니다.   

✅ 참조 링크
```md
[링크 키워드][id]  <!-- 링크를 참조 방식으로 설정 -->

[id]: URL "선택적 제목 여기"  <!-- 참조할 링크의 실제 URL을 정의 -->

/*
Markdown에서 참조 스타일 링크를 사용하는 방법:
1. `[링크 키워드][id]` 형식으로 링크를 작성합니다.
2. `[id]: URL "선택적 제목"` 형식으로 링크의 대상(URL)을 정의합니다.
3. 제목("선택적 제목") 부분은 마우스를 올렸을 때 표시되는 툴팁이며 생략 가능함.

예시:
[구글][google]

[google]: https://www.google.com "이곳을 누르면 구글로 이동합니다."
*/
```
## 결과값

[구글][google]

[google]: https://www.google.com "이곳을 누르면 구글로 이동합니다."

✅ 직접 링크

```md
Markdown에서 직접 링크를 추가하는 방법:
1. `[텍스트](URL "선택적 제목")` 형식으로 작성합니다.
2. `텍스트` 부분은 클릭 가능한 링크의 이름입니다.
3. `URL` 부분은 이동할 웹사이트 주소입니다.
4. `"선택적 제목"` 부분은 마우스를 올렸을 때 표시되는 툴팁이며 생략 가능함.

예시:
[네이버](https://www.naver.com "네이버 링크")
```


## 결과값
[네이버](https://www.naver.com "이곳을 누르면 네이버로 이동합니다.")

✅ 자동 연결 (Autolinks)   
일반적인 URL 혹은 이메일 주소는 자동으로 링크로 변환됩니다.
```md
* 외부링크: <http://example.com/>
* 이메일링크: <address@example.com>
```

## 결과값

* 외부링크: <http://example.com/>
* 이메일링크: <address@example.com>

---

### ✅ 강조
Markdown에서는 텍스트를 굵게(Bold), 기울임체(Italic), 취소선 으로 강조할 수 있습니다.

```md
*single asterisks*
_single underscores_
**double asterisks**
__double underscores__
~~cancelline~~
```

## 결과값

*single asterisks*   
_single underscores_   
**double asterisks**   
__double underscores__   
~~cancelline~~   

### ✅ 이미지 (Image)
Markdown에서 이미지를 삽입하는 방법입니다.   
✅ 기본 이미지 삽입
```md
![대체 텍스트](/path/to/img.jpg)  
![대체 텍스트](/path/to/img.jpg "선택적 제목")

Markdown에서 이미지 삽입하는 방법:
1. `![대체 텍스트](이미지 경로)` 형식으로 작성합니다.
2. `대체 텍스트`는 이미지가 로드되지 않을 때 표시되는 텍스트입니다.
3. `이미지 경로`는 이미지 파일의 URL 또는 파일 경로입니다.
4. `"선택적 제목"`을 추가하면 마우스를 올렸을 때 툴팁이 표시됩니다.

예시:
![고양이 이미지](https://flexible.img.hani.co.kr/flexible/normal/765/459/imgdb/child/2024/0607/53_17177430334988_20240607501743.webp "귀여운 고양이")
```

## 결과값

![고양이 이미지](https://flexible.img.hani.co.kr/flexible/normal/765/459/imgdb/child/2024/0607/53_17177430334988_20240607501743.webp "귀여운 고양이")

✅ Markdown에서는 이미지 크기 조절 기능이 없음   

Markdown 자체적으로는 이미지의 크기를 조절할 수 없습니다.   
HTML 태그 <img>를 사용하면 크기를 조절할 수 있습니다.

```md
<!-- HTML을 사용하여 이미지 크기를 조절하는 방법 -->
<img src="/path/to/img.jpg" width="450px" height="300px" title="px(픽셀) 크기 설정" alt="고양이"><br/>
<img src="/path/to/img.jpg" width="40%" height="30%" title="비율 크기 설정" alt="고양이">

Markdown에서는 기본적으로 이미지 크기 조절 기능이 없기 때문에,
HTML `<img>` 태그를 사용하여 크기를 직접 설정할 수 있습니다.

1. `src="/path/to/img.jpg"` → 이미지 파일 경로 또는 URL
2. `width="450px" height="300px"` → 픽셀 단위로 크기 설정
3. `width="40%" height="30%"` → 화면 크기에 대한 비율(%)로 조절 가능
4. `title="설명"` → 마우스를 올렸을 때 표시되는 툴팁
5. `alt="대체 텍스트"` → 이미지가 로드되지 않을 경우 표시될 텍스트
```

## 결과값

<img src="https://flexible.img.hani.co.kr/flexible/normal/765/459/imgdb/child/2024/0607/53_17177430334988_20240607501743.webp" width="300px" height="200px" alt="고양이">

---

✅ 줄바꿈
Markdown에서 줄 바꿈을 제대로 적용하려면   
+ 문장 끝에 스페이스 2개   
+ HTML ```<br>``` 태그 사용   
+ 빈 줄 추가   

```
줄 바꿈을 하기 위해서는 문장 마지막에서 3칸이상을 띄어쓰기해야 한다.   이렇게

줄 바꿈을 하기 위해서는 문장 마지막에서 3칸이상을 띄어쓰기해야 한다. <br> 이렇게

줄 바꿈을 하기 위해서는 문장 마지막에서 3칸이상을 띄어쓰기해야 한다.

이렇게
```
## 결과값

줄 바꿈을 하기 위해서는 문장 마지막에서 3칸이상을 띄어쓰기해야 한다.   이렇게

줄 바꿈을 하기 위해서는 문장 마지막에서 3칸이상을 띄어쓰기해야 한다. <br> 이렇게

줄 바꿈을 하기 위해서는 문장 마지막에서 3칸이상을 띄어쓰기해야 한다.

이렇게
