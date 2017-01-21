---
layout: post
title: third post
---

## 개발환경 구축

### JDK 설치

1. [JDK 다운로드](http://www.oracle.com/technetwork/java/javase/downloads/index.html)

2. 설치 `C:\Java\jdk1.8.0_121\`

3. 환경변수 설정

`JAVA_HOME` = `C:\Java\jdk1.8.0_121`

`path` = `%JAVA_HOME%\bin;%path%`

### Eclipse 설정

1. 이클립스 javaEE Developers 버전 다운로드 [http://eclipse.org](http://www.eclipse.org/downloads/eclipse-packages/)

2. 압출 풀고 실행

3. 워크스페이스 폴더 선택

4. Encoding 설정 : `window > preference` > enc로 검색 > UTF-8로 설정
 
	- General > Contents Types > Text > Default encoding
	- General > Contents Types > Text > JSP > Default encoding
	- General > Workspace > Text file encoding
	- Web > CSS Files > Encoding
	- Web > HTML Files > Encoding
	- Web > JSP Files > Encoding
	- XML > XML Files > Encoding

5. 기본 Folding 해제 : `window > preference` > folding로 검색
	- Java > Editor > Folding > 전부 체크해제(Enable 제외)
	- Java > Editor > Folding > 전부 체크해제(Enable 제외)

6. JRE 재확인  : `window > preference > java > Installed JRE > JDK > edit` (%JAVA_HOME% 경로설정을 제대로 해야 addd안에서 JDK를 확인할 수 있다.)
	- rt.jar > Javadoc location (URL -> Archive로 경로 변경) 
		Archivep path : `jdk-8u121-docs-all.zip`
        Path within archive : `docs/api`

7. Font 설정 : `window > General > Color and Fonts > Basic > Text Font, Text Editor Block Selection Font`
	- 나눔고딕, D2 Coding 글씨체 추천

8. Code Style format 설정 : 
	Import > `window > Java > Code Style > Formatter > Import `
    Export > `window > Java > Code Style > Formatter > Edit > 변경후 Export `
    cf) 단축키 : `ctrl + shift + f`
    tip) 저장 시 자동 Formatting : `window > preference > Java > Editor > Save ACtions > Perform the selected... 체크, Format source code 체크 확인

9. Spelling 기능 해제

10. View 설정 : Quick Access(ctrl + 3) > pakage Explorer, Navigator, Tasks, Javadoc
	- Package Explorer : 보기 간편하기 때문에 사용하면 용이하다
	- Navigator : Project Explorer나 Package Explorer에서 볼 수 없는 설정 파일(숨김파일)을 표시 cf) Navigator에서 파일명 변경 시 source가 자동으로 바뀌지 않는다.
	- Tasks : //TODO 확인
	- Javadoc : Javadcc 확인

11. Server에 Tomcat 추가 : View > Servers > new > server > Apache > Tom/Cat 버전 확인 > Bowser > Tomcat 디렉토리 선택 (bin으로 들어가지 않는다.) cf) Dynamic Web Project 생성 시 Target Runtime에 Apache Tomcat이 자동으로 선택되지 않는다.
오류잡는 법 : 
`Project > Properties > Java Build Path > Libraries > Add Library > Server Runtime > 서버 선택`


### github 설치






