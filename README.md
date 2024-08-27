# 프로젝트 이름 : AI를 활용한 CBT 문제 생성기

## 제안 배경 
> 기존의 CBT(Computer-Based Testing) 시스템은 주로 일률적인 문제 출제와 평가 방식을 제공해왔지만, 학습자의 개별적인 요구를 충분히 반영하지 못하는 한계가 있었습니다. 그러나 AI 기술의 발전으로 맞춤형 문제 출제와 학습 지원이 가능해지면서, 개인화된 학습 경험을 제공하는 혁신적인 플랫폼이 등장하고 있습니다. 이 플랫폼은 학습자의 이해도를 높이고, 반복 학습과 실시간 피드백을 통해 학습 효과를 극대화하며, 학습 과정 전반을 효율적으로 관리할 수 있도록 지원합니다.

## 프로젝트 기능
- **맞춤형 문제 출제**
  - 사용자는 자신의 학습 진도에 따라 개인 맞춤형 문제를 자동으로 제공받을 수 있습니다.
  - **챌린지 포인트 (외부 API 사용)**: ChatGPT를 이용한 문제 생성 기능 구현.
    1. 출력할 값의 형태를 문제 형식으로 정리하여 제공.
    2. 생성된 문제를 사용자 화면에 출력.
- **실시간 성적 분석**
  - 시험 후 즉시 성적 분석을 받아 자신의 학습 상태를 확인할 수 있습니다.
- **맞춤형 피드백**
  - 학습 과정에서 발생한 약점에 대한 피드백을 제공받아, 개선이 필요한 부분을 집중적으로 학습할 수 있습니다.
- **SNS 로그인**
  - 카카오 로그인 기능을 통해 사용자 편의성을 높입니다.
  - **챌린지 포인트 (SNS 로그인)**: 카카오 오픈 로그인 API를 활용한 로그인 기능 구현.
    1. 오픈 로그인 API 이용 신청.
    2. CLIENT_ID와 REDIRECT_URL 등록.
    3. 카카오 로그인 버튼 생성.
    4. 카카오 로그인 POPUP 설정.
    5. API를 통해 이메일, 닉네임, 엑세스 토큰 받아오기.

## 구현 기능
- **AI 기반 문제 생성 엔진**
  - ChatGPT를 활용하여 학습 데이터를 분석하고, 사용자 맞춤형 문제를 생성하는 엔진.
  - 생성된 문제를 화면에 출력하는 기능.
- **성적 분석 알고리즘**
  - 실시간으로 학습자의 시험 데이터를 처리하여 성적을 분석하고 피드백을 제공하는 알고리즘.
- **SNS 로그인 연동**
  - 카카오 오픈 로그인 API를 이용하여 SNS 로그인 기능 구현.
  - 사용자 이메일, 닉네임, 엑세스 토큰을 API를 통해 받아오는 기능.
- **인터페이스 디자인**
  - 사용자가 학습 진도와 피드백을 직관적으로 확인할 수 있는 사용자 인터페이스(UI) 설계.

## 세부 기능
- **문제 생성**
  - AI 기반 문제 생성 엔진을 통해 학습자의 이해도에 맞춘 문제를 생성.
- **문제 풀이**
  - 생성된 문제를 사용자가 풀이할 수 있도록 화면에 제공.
- **오답 노트**
  - 사용자가 틀린 문제를 저장하고, 복습할 수 있도록 기능 제공.
- **사용자 분석**
  - 성적 분석 알고리즘을 통해 학습자의 강점과 약점을 분석하여 제공.

### 📎 팀명: 코드커버리
<img src="https://fpcedu.co.kr/2024smhrd/%ed%95%b5%ec%8b%ac%ec%9c%b5%ed%95%a9%ed%94%84%eb%a1%9c%ec%a0%9d%ed%8a%b8-%ec%bd%94%eb%93%9c%ec%bb%a4%eb%b2%84%eb%a6%ac/GitHUB_imgs/CodeCoveryLogo.png" alt="codecovery_logo" width="200"/>

### 👀 서비스 소개
- **서비스명**: AI를 활용한 CBT 문제 생성기
- **서비스 설명**: 유저가 웹사이트에 데이터를 입력(질문, 파일 업로드, 풀었던 문제)하면, Computer-Based Testing 형식의 문제를 생성하여 제공합니다. 사용자는 생성된 문제를 바로 풀어보고, 실시간으로 채점 결과를 받을 수 있습니다.

### 📅 프로젝트 기간
- **2024.07.16 ~ 2024.08.26 (7주)**

### ⭐ 주요 기능
- **맞춤형 문제 생성**
  - **AI 기반 문제 생성**: ChatGPT를 활용하여 학습자의 입력 데이터를 분석하고, 개인 맞춤형 문제를 자동으로 생성합니다. 문제는 학습자의 이해도와 학습 진도에 맞추어 난이도가 조절되며, 다양한 문제 유형이 제공됩니다.
  - **출력 형식 설정**: 생성된 문제를 Computer-Based Testing(CBT) 형식에 맞게 자동으로 포맷팅하여 출력합니다.
- **실시간 성적 분석**
  - **자동 채점**: 사용자가 푼 문제를 즉시 채점하여 성적을 제공합니다. 채점 결과는 실시간으로 피드백되며, 사용자는 자신의 학습 상태를 즉각적으로 파악할 수 있습니다.
- **맞춤형 피드백**
  - **개인화된 피드백 제공**: 채점 결과를 기반으로 학습자의 약점을 분석하고, 해당 부분에 대한 맞춤형 피드백을 제공합니다. 피드백을 통해 학습자는 개선이 필요한 부분을 집중적으로 학습할 수 있습니다.
  - **오답 노트 기능**: 사용자가 틀린 문제를 자동으로 저장하고, 복습할 수 있는 기능을 제공합니다. 이를 통해 반복 학습이 가능하며, 학습자의 장기 기억 형성을 돕습니다.
- **SNS 로그인**
  - **카카오 로그인**: 카카오 오픈 로그인 API를 이용하여 간편하게 웹사이트에 로그인할 수 있는 기능을 제공합니다. 이를 통해 사용자는 별도의 회원가입 없이 손쉽게 서비스에 접근할 수 있습니다.
- **사용자 인터페이스(UI) 및 사용자 경험(UX)**
  - **직관적이고 사용자 친화적인 UI 설계**: 사용자가 쉽게 접근하고 사용할 수 있도록 직관적이고 심플한 인터페이스를 설계합니다.

### ⛏ 기술스택
<table>
  <tr>
    <td style="width: 15%; vertical-align: top;">
      <img src="https://fpcedu.co.kr/2024smhrd/%ed%95%b5%ec%8b%ac%ec%9c%b5%ed%95%a9%ed%94%84%eb%a1%9c%ec%a0%9d%ed%8a%b8-%ec%bd%94%eb%93%9c%ec%bb%a4%eb%b2%84%eb%a6%ac/GitHUB_imgs/eclipse.png" alt="Eclipse" style="width: 50px;">
    </td>
    <td style="width: 85%; vertical-align: top;">
      <b>IDE</b> : Eclipse(2024-06)
    </td>
  </tr>
  <tr>
    <td style="width: 15%; vertical-align: top;">
      <img src="https://fpcedu.co.kr/2024smhrd/%ed%95%b5%ec%8b%ac%ec%9c%b5%ed%95%a9%ed%94%84%eb%a1%9c%ec%a0%9d%ed%8a%b8-%ec%bd%94%eb%93%9c%ec%bb%a4%eb%b2%84%eb%a6%ac/GitHUB_imgs/maven.png" alt="Maven" style="width: 50px;">
    </td>
    <td style="width: 85%; vertical-align: top;">
      <b>프로젝트 관리 및 빌드</b> : Maven(v3.8.1)
    </td>
  </tr>
  <tr>
    <td style="width: 15%; vertical-align: top;">
      <img src="https://fpcedu.co.kr/2024smhrd/%ed%95%b5%ec%8b%ac%ec%9c%b5%ed%95%a9%ed%94%84%eb%a1%9c%ec%a0%9d%ed%8a%b8-%ec%bd%94%eb%93%9c%ec%bb%a4%eb%b2%84%eb%a6%ac/GitHUB_imgs/jsp_servlet.png" alt="JSP & Servlet" style="width: 50px;">
    </td>
    <td style="width: 85%; vertical-align: top;">
      <b>웹 애플리케이션 개발</b> : JSP, Servlet, MVC패턴
    </td>
  </tr>
  <tr>
    <td style="width: 15%; vertical-align: top;">
      <img src="https://fpcedu.co.kr/2024smhrd/%ed%95%b5%ec%8b%ac%ec%9c%b5%ed%95%a9%ed%94%84%eb%a1%9c%ec%a0%9d%ed%8a%b8-%ec%bd%94%eb%93%9c%ec%bb%a4%eb%b2%84%eb%a6%ac/GitHUB_imgs/oracle.png" alt="Oracle" style="width: 50px;">
    </td>
    <td style="width: 85%; vertical-align: top;">
      <b>데이터베이스</b> : Oracle (ojdbc8 v21.1.0.0)
    </td>
  </tr>
  <tr>
    <td style="width: 15%; vertical-align: top;">
      <img src="https://fpcedu.co.kr/2024smhrd/%ed%95%b5%ec%8b%ac%ec%9c%b5%ed%95%a9%ed%94%84%eb%a1%9c%ec%a0%9d%ed%8a%b8-%ec%bd%94%eb%93%9c%ec%bb%a4%eb%b2%84%eb%a6%ac/GitHUB_imgs/mybatis.png" alt="MyBatis" style="width: 50px;">
    </td>
    <td style="width: 85%; vertical-align: top;">
      <b>ORM 프레임워크</b> : MyBatis (v3.5.6)
    </td>
  </tr>
  <tr>
    <td style="width: 15%; vertical-align: top;">
      <img src="https://fpcedu.co.kr/2024smhrd/%ed%95%b5%ec%8b%ac%ec%9c%b5%ed%95%a9%ed%94%84%eb%a1%9c%ec%a0%9d%ed%8a%b8-%ec%bd%94%eb%93%9c%ec%bb%a4%eb%b2%84%eb%a6%ac/GitHUB_imgs/lombok.png" alt="Lombok" style="width: 50px;">
    </td>
    <td style="width: 85%; vertical-align: top;">
      <b>코드 간소화</b> : Lombok (v1.18.34)
    </td>
  </tr>
  <tr>
    <td style="width: 15%; vertical-align: top;">
      <img src="https://fpcedu.co.kr/2024smhrd/%ed%95%b5%ec%8b%ac%ec%9c%b5%ed%95%a9%ed%94%84%eb%a1%9c%ec%a0%9d%ed%8a%b8-%ec%bd%94%eb%93%9c%ec%bb%a4%eb%b2%84%eb%a6%ac/GitHUB_imgs/tomcat.png" alt="Apache Tomcat" style="width: 50px;">
    </td>
    <td style="width: 85%; vertical-align: top;">
      <b>서버</b> : Apache Tomcat (9.0.91) Local Server
    </td>
  </tr>
  <tr>
    <td style="width: 15%; vertical-align: top;">
      <img src="https://fpcedu.co.kr/2024smhrd/%ed%95%b5%ec%8b%ac%ec%9c%b5%ed%95%a9%ed%94%84%eb%a1%9c%ec%a0%9d%ed%8a%b8-%ec%bd%94%eb%93%9c%ec%bb%a4%eb%b2%84%eb%a6%ac/GitHUB_imgs/git.png" alt="Git" style="width: 50px;">
    </td>
    <td style="width: 85%; vertical-align: top;">
      <b>버전 관리</b> : Git
    </td>
  </tr>
  <tr>
    <td style="width: 15%; vertical-align: top;">
      <img src="https://fpcedu.co.kr/2024smhrd/%ed%95%b5%ec%8b%ac%ec%9c%b5%ed%95%a9%ed%94%84%eb%a1%9c%ec%a0%9d%ed%8a%b8-%ec%bd%94%eb%93%9c%ec%bb%a4%eb%b2%84%eb%a6%ac/GitHUB_imgs/log4j.png" alt="Log4j" style="width: 50px;">
    </td>
    <td style="width: 85%; vertical-align: top;">
      <b>로그 관리</b> : Log4j (v1.2.17)
    </td>
  </tr>
</table>

### 기능
|  |  |
|:---:|---|
|  | **Json 처리**: Apache HttpClient(v5.1), Gson(v2.8.9) - JSON 파일의 직렬화 및 역직렬화를 위한 라이브러리 |
|  | **파일 처리**: 문서 파일 처리 및 분석을 위해 Tika와 HWP 라이브러리 사용 (tika-core v2.9.2, tika-parsers-standard-package v2.9.2, kr.dogfoot.hwplib v1.1.6) |
|  | **키워드 추출**: Korean Summarizer (com.github.tuguri8 v0.1.2) |

### 테스트 및 빌드
|  |  |
|:---:|---|
|  | **테스트 프레임워크**: JUnit (v4.11) |
|  | **패키징**: Maven War Plugin(v3.2.3) |


### ⚙ 시스템 아키텍처(구조)
![시스템 아키텍쳐-코드커버리팀](https://fpcedu.co.kr/2024smhrd/%ed%95%b5%ec%8b%ac%ec%9c%b5%ed%95%a9%ed%94%84%eb%a1%9c%ec%a0%9d%ed%8a%b8-%ec%bd%94%eb%93%9c%ec%bb%a4%eb%b2%84%eb%a6%ac/GitHUB_imgs/systemArchitecture.jpg)

### 📌 SW유스케이스
![코드커버리_유스케이스](https://fpcedu.co.kr/2024smhrd/%ed%95%b5%ec%8b%ac%ec%9c%b5%ed%95%a9%ed%94%84%eb%a1%9c%ec%a0%9d%ed%8a%b8-%ec%bd%94%eb%93%9c%ec%bb%a4%eb%b2%84%eb%a6%ac/GitHUB_imgs/usecase.png)

### 📌 서비스 흐름도
![코드커버리_서비스흐름도](https://fpcedu.co.kr/2024smhrd/%ed%95%b5%ec%8b%ac%ec%9c%b5%ed%95%a9%ed%94%84%eb%a1%9c%ec%a0%9d%ed%8a%b8-%ec%bd%94%eb%93%9c%ec%bb%a4%eb%b2%84%eb%a6%ac/GitHUB_imgs/service_flow.jpg)

### 📌 ER다이어그램
![코드커버리_ER다이어그램](https://fpcedu.co.kr/2024smhrd/%ed%95%b5%ec%8b%ac%ec%9c%b5%ed%95%a9%ed%94%84%eb%a1%9c%ec%a0%9d%ed%8a%b8-%ec%bd%94%eb%93%9c%ec%bb%a4%eb%b2%84%eb%a6%ac/GitHUB_imgs/erdiagram.png)

### 🖥 화면 구성
![메인화면](https://fpcedu.co.kr/2024smhrd/%ed%95%b5%ec%8b%ac%ec%9c%b5%ed%95%a9%ed%94%84%eb%a1%9c%ec%a0%9d%ed%8a%b8-%ec%bd%94%eb%93%9c%ec%bb%a4%eb%b2%84%eb%a6%ac/GitHUB_imgs/screen%20(5).jpg)
![비로그인_팝업](https://fpcedu.co.kr/2024smhrd/%ed%95%b5%ec%8b%ac%ec%9c%b5%ed%95%a9%ed%94%84%eb%a1%9c%ec%a0%9d%ed%8a%b8-%ec%bd%94%eb%93%9c%ec%bb%a4%eb%b2%84%eb%a6%ac/GitHUB_imgs/screen%20(6).jpg)
![로그인_팝업](https://fpcedu.co.kr/2024smhrd/%ed%95%b5%ec%8b%ac%ec%9c%b5%ed%95%a9%ed%94%84%eb%a1%9c%ec%a0%9d%ed%8a%b8-%ec%bd%94%eb%93%9c%ec%bb%a4%eb%b2%84%eb%a6%ac/GitHUB_imgs/screen%20(7).jpg)
![로그인](https://fpcedu.co.kr/2024smhrd/%ed%95%b5%ec%8b%ac%ec%9c%b5%ed%95%a9%ed%94%84%eb%a1%9c%ec%a0%9d%ed%8a%b8-%ec%bd%94%eb%93%9c%ec%bb%a4%eb%b2%84%eb%a6%ac/GitHUB_imgs/screen%20(8).jpg)
![회원가입](https://fpcedu.co.kr/2024smhrd/%ed%95%b5%ec%8b%ac%ec%9c%b5%ed%95%a9%ed%94%84%eb%a1%9c%ec%a0%9d%ed%8a%b8-%ec%bd%94%eb%93%9c%ec%bb%a4%eb%b2%84%eb%a6%ac/GitHUB_imgs/screen%20(9).jpg)
![회원탈퇴](https://fpcedu.co.kr/2024smhrd/%ed%95%b5%ec%8b%ac%ec%9c%b5%ed%95%a9%ed%94%84%eb%a1%9c%ec%a0%9d%ed%8a%b8-%ec%bd%94%eb%93%9c%ec%bb%a4%eb%b2%84%eb%a6%ac/GitHUB_imgs/screen%20(10).jpg)
![문제풀이](https://fpcedu.co.kr/2024smhrd/%ed%95%b5%ec%8b%ac%ec%9c%b5%ed%95%a9%ed%94%84%eb%a1%9c%ec%a0%9d%ed%8a%b8-%ec%bd%94%eb%93%9c%ec%bb%a4%eb%b2%84%eb%a6%ac/GitHUB_imgs/screen%20(11).jpg)
![질의응답](https://fpcedu.co.kr/2024smhrd/%ed%95%b5%ec%8b%ac%ec%9c%b5%ed%95%a9%ed%94%84%eb%a1%9c%ec%a0%9d%ed%8a%b8-%ec%bd%94%eb%93%9c%ec%bb%a4%eb%b2%84%eb%a6%ac/GitHUB_imgs/screen%20(12).jpg)
![질의응답게시글](https://fpcedu.co.kr/2024smhrd/%ed%95%b5%ec%8b%ac%ec%9c%b5%ed%95%a9%ed%94%84%eb%a1%9c%ec%a0%9d%ed%8a%b8-%ec%bd%94%eb%93%9c%ec%bb%a4%eb%b2%84%eb%a6%ac/GitHUB_imgs/screen%20(13).jpg)

### 👨‍👩‍👦‍👦 팀원역할
| 역할         | 이름          | 담당 업무                        |
| ------------ | ------------- | -------------------------------- |
| **팀장 (PM)**  | 김도영        | 프로젝트 매니지먼트 (PM)        |
| **팀원**      | 배준규        | Back-end 개발,DB                 |
| **팀원**      | 이송희        | Front-end 개발                   |
| **팀원**      | 허재혁        | Back-end 개발                    |

### 🤾‍♂️ 트러블슈팅
개념: 문제 해결을 위해 문제의 원인을 논리적이고 체계적으로 찾는 일이며 제품이나 프로세스의 운영을 재개 프로젝트 진행하는 동안 발생했던 이슈 중 가장 기억에 남았던 문제와 해결 프로세스 나열(2~5가지 정도)

문제1
회원가입 폼과 회원수정 폼을 같이 쓰다가 로그인을 확인하는 부분에서 오류가 나서 서로 분리하여 해

문제2
문제점 설명 및 해결방안
