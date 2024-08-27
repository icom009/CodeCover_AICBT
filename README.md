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
| **팀원**      | 배준규        | Back-end 개발,DB                |
| **팀원**      | 이송희        | Front-end 개발                   |
| **팀원**      | 허재혁        | Back-end 개발,DB                    |

### 🤾‍♂️ 트러블슈팅
- 문제: 문제 은행(DB -> TB_GENERATED_QUESTION)에서 사용자 키워드 검색 시, 영어와 한글이 섞여서 존재하여 검색 결과가 불완전하게 나오는 문제가 발생.
> 해결방안: 한글로 검색하든 영어로 검색하든, 번역된 결과도 함께 검색할 수 있도록 개선. MakeTestController(Servlet)에서 `/src/main/resources/translate.py` 파이썬 파일을 실행해 검색 키워드를 번역(구글트랜스 라이브러리 사용)하여 DB 검색에 사용. 한글 깨짐 문제는 UTF-8 적용으로 해결.
- 문제: 키워드 기반 검색을 위한 NLP 처리가 필요했으나, 어떤 NLP를 사용할지 결정되지 않아 기능 완성이 지연됨. 예를 들어, "JAVA 문제가 필요해"와 같은 문장에서 "JAVA"와 같은 키워드를 추출해야 함.
> 해결방안: MVN Korean Trigger 라이브러리를 사용하여 한글 키워드 추출 문제를 해결함.
- 문제: 외부 SNS 계정(네이버, 카카오, 구글) 로그인 기능을 구현하는 과정에서, 각 서비스마다 가져올 수 있는 사용자 정보가 다르고, 로그인 흐름이 복잡하여 통합 관리가 어려웠음.
> 해결방안: 각 SNS별로 필요한 애플리케이션 등록 및 설정을 완료한 후, 로그인 시 사용자의 snsid와 snstype 정보를 DB에 저장하고 이를 기준으로 회원가입 여부를 확인. 회원가입이 필요한 경우, 회원가입 폼을 작성하여 필요한 정보를 추가로 입력받고, 세션에 정보를 저장한 후 메인 화면으로 이동. 네이버, 카카오, 구글 모두 동일한 흐름으로 처리하며, 사용자가 로그인 시 SNS 로그인 기능을 통해서만 로그인하도록 설정.
- 문제: 파일 업로드를 통한 문제 생성 기능을 구현하는 과정에서, 파일 이름 중복 처리, 다양한 파일 형식의 텍스트 추출, 그리고 텍스트 전처리에 대한 문제들이 발생함.
> 해결방안: 파일 업로드 컨트롤러에서 파일 이름 중복 시 `_1, _2, _3`과 같이 번호를 추가하여 저장하도록 구현. HWP 및 PDF 파일에서 텍스트를 추출하기 위해 각각 `hwplib` 라이브러리와 `tesseract`를 사용하여 OCR 처리를 진행. 추출된 텍스트는 `NoriAnalyzer`로 전처리하였으나, 복잡한 전처리 대신 기본적인 `\n` 처리 후, 핵심 키워드 5개를 추출하여 ChatGPT로 전달하는 방식으로 문제를 해결함.
- 문제: ChatGPT 무료화를 위해 오픈소스 GPT-2를 활용하려 했으나, 모델 교육에 시간이 너무 많이 소요되고 성능이 기대에 미치지 못함. Colab에서는 10시간 이상, 맥북에서는 46시간 이상 소요됨.
> 해결방안: Colab Pro 버전(A100 GPU 사용)을 결제하여 모델 교육 시간을 2시간 30분으로 단축했으나, 여전히 성능이 부족하고 영어만 인식하는 등의 한계가 있어, GPT-2 대신 GPT-3.5를 저렴한 가격에 사용하는 것으로 방향을 변경.
- 문제: 회원가입과 정보수정 페이지에서 동일한 JSP 파일을 공유하면서, 회원정보 수정 시 비동기 통신 기능이 제대로 작동하지 않는 문제가 발생.
> 해결방안: 회원정보 수정 전용 form을 별도로 만들어 비동기 통신 기능이 정상적으로 작동하도록 문제를 해결함.


