# 🚀 Makefile 직접 만들어보기 실습

## (실습 교재는 아직 준비 중입니다.)
## 기본적인 컴파일 단계
## 기본적인 gcc 명령 사용법
## 기본적인 Make 규칙

```Makefile
Target : Dependency
    Recipe
```

### 모든 것은 여기에 [GNU 메이크파일 메뉴얼](https://www.gnu.org/software/make/manual/make.html)
- Make는 첫번 째 target에서 시작한다. 이 target을 defalut target 이라고 한다.
- [자동 변수(Automatic Variables)](https://www.gnu.org/software/make/manual/make.html#Automatic-Variables)
- [메이크파일 내의 조건문](https://www.gnu.org/software/make/manual/make.html#Conditional-Syntax)
- [기본  변수(Variables used by implicit Rules)](https://www.gnu.org/software/make/manual/make.html#Implicit-Variables)
- [긴 줄 쪼개기](https://www.gnu.org/software/make/manual/make.html#Splitting-Lines)
- [.c.o 올드 스타일](https://www.gnu.org/software/make/manual/make.html#Suffix-Rules)
- [암시적인 규칙](https://www.gnu.org/software/make/manual/make.html#Catalogue-of-Rules)
- [포니 타겟](https://www.gnu.org/software/make/manual/make.html#Phony-Targets)
- [Addprefix](https://www.gnu.org/software/make/manual/make.html#Text-Functions)
- c프로젝트 디렉토리 구조
---

참고 자료 : [Make에 대해 알아야 할 7가지](https://www.mimul.com/blog/7-things-you-should-know-about-make/)

Q. 메이크파일에는 default 로 세팅되어있는 컴파일 규칙이 있다

Q. 접미사 규칙 vs 패턴 규칙
