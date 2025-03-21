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
# This is a H1
## This is a H2
### This is a H3
#### This is a H4
##### This is a H5
###### This is a H6

```
## 결과값

# This is a H1
## This is a H2
### This is a H3
#### This is a H4
##### This is a H5
###### This is a H6
---
### ✅ BlockQuote (인용문)
이메일에서 사용하는 > 기호를 활용하여 인용문을 작성할 수 있습니다.

```md
> This is a first blockqute.
>	> This is a second blockqute.
>	>	> This is a third blockqute.
```

## 결과값
> This is a first blockquote.
>	> This is a second blockquote.
>	>	> This is a third blockquote.
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

### ✅ * 혼합된 목록 (Nested List)
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

### ✅ 코드 블록 (Indentation & Code Blocks)
Markdown에서 들여쓰기(Indentation) 를 사용하면 코드 블록이 생성됩니다.
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
---
✅ 방법 2: 백틱(```)을 이용

```java
public class BootSpringBootApplication {
  public static void main(String[] args) {
    System.out.println("Hello, JB");
  }
}
```
