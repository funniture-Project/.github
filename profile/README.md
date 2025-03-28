
![image](https://github.com/user-attachments/assets/a37e3b69-4c2d-4cff-9f62-1230b8891e70)
<br/>

# **프로젝트 : <span align="flex-start"><img src="https://github.com/user-attachments/assets/de1c42b1-253c-4ea2-b67c-2d1a9a101bf2" alt="로고" width="230px" hegih="150px"></span>**
<spqn>🕒 **2025.01.13 ~ 2025.03.17 (9주)**</span>
| 📃 [Notion](https://www.notion.so/ohgiraffers/Funniture-a20b3bd6541044bb92633168355e984d) | 🎨 [Figma](https://www.figma.com/design/LerWvqtQYoZsDC5apYe5R4/Funniture?node-id=0-1&p=f&t=H87Z57FzWKf1Kxf2-0) | 
<br/>
<br/>

## 📋개요
이 프로젝트는 가구 및 가전 제품의 렌탈 서비스를 제공하는 **Funniture** 플랫폼입니다.<br/>
단순 대여 서비스를 넘어 렌탈부터 반납까지 관리하여 사용자와 제공자 모두에게 편리한 **원스톱 관리 서비스**를 제공하고 있습니다.<br/>
고객이 가전과 가구를 통해 새로운 즐거움과 편리함을 경험하길 바라는 마음을 담아 <br/>
프로젝트의 이름을 **재미(fun)** 와 **가구(furniture)** 를 결합하여 만들었습니다.<br/>

## 👨‍👧‍👧팀원 소개

| 이름     | 이미지                                                                 | 역할     | 기능개발                                                        |
|----------|-----------------------------------------------------------------------|----------|-----------------------------------------------------------------|
| 정예진   | <p align="center"><img src="https://github.com/user-attachments/assets/a9a3ca81-96a4-4fb2-b108-f01a7551f011" height="100" textalign="center"></p> | PM       | 챗봇, 상품관리, 관심상품, 최근본상품, 관리자 문의, 공지사항 |
| 정은미   | <img src="https://github.com/user-attachments/assets/b237ab0e-2221-4811-8f4d-6407a88f408e" width="130" height="100"> | 형상관리자 | 배송지, 포인트, 예약관리, 반납관리, 매출 및 정산 |
| 김규남   | <img src="https://github.com/user-attachments/assets/b26bacbc-7dd4-4798-a365-5c1e1386ecf6" width="130" height="100"> | DBA      | 로그인, 회원가입, 회원관리, 리뷰, 제공자 1:1 문의 |

## 🖥 기술 스택

| 구분                 | 사용 기술 및 라이브러리          |
| -------------------- | ------------------------------- |
| 언어                 |  Java, JavaScript               |
| 프레임워크             | Spring Boot, React            |
| DBMS 및 ORM         |  MySQL                           |
| 백엔드    | Spring Security, Swagger, Cloudinary, Query DSL, JPA  |
| 프론트엔드    | React-Bootstrap, ApexChart.js, Redux, Axios, React-Quill |

## 🌟주요 기능

### <공통>
**1. 회원가입(규남)**<br/>

**2. 상품정보(예진)**<br/>

**3. 로그인(규남)**<br/>

**4. ✅챗봇(예진)✅**<br/>

▶ 일반 챗봇 사용
![usedchatbot](https://github.com/user-attachments/assets/b7fe55cb-d8c5-4a18-8429-e053437cd2dc)
- 챗봇은 회원가입의 유무와 관련 없이 사용가능하며, 하위 질문 여부와 관리자 연결여부에 따라 다음 출력되는 내용들을 구성.
- 관리자 연결을 원할 시에는 로그인여부를 파악하여 연결 가능 여부 출력
- 처음 질문 리스트와 이전 선택 질문 번호를 저장하기위해 useRef 사용

<br/>

### <사용자>
**1. 메인(예진)**<br/>

**2. 회원정보 변경(규남)**<br/>

**3. 제공자 전환 신청(규남)**<br/>

**4. 배송지 관리(은미)**<br/>
![배송지관리](https://github.com/user-attachments/assets/a352f088-10a8-4695-8c84-87a5b67c780b)

- 신규 배송지 등록&수정&삭제 기능(다음 주소검색 API 사용)
- 기본 배송지로 선택

**5. 주문/배송(은미)**<br/>

**6. 사용상품/반납(은미)**<br/>

**7. 관심 상품(예진)**<br/>

**8. 최근 본 상품(예진)**<br/>

**9. 리뷰(규남)**<br/>

**10. 1:1 문의(예진)**<br/>
<br/>

### <제공자>
**1. 메인(공동)**<br/>

**2. 사업자 정보(규남)**<br/>

**3. 상품 등록 및 수정(예진)**<br/>
![상품 등록](https://github.com/user-attachments/assets/30a00017-878a-432d-a128-b46de91034ca)

- 상품 정보 등록에 react-quill을 적용하여 제공자에게 자유로운 콘텐츠 작성과 예측 가능성제공
- 대표 이미지 및 상품 설명내의 이미지 데이터 cloudinary를 이용하여 처리
- 렌탈 개월수에 따른 가격 및 as횟수 등록 가능

**4. 상품 상태 변경(예진)**<br/>
![상품 상태 변경](https://github.com/user-attachments/assets/80d3b4c5-85bb-4729-9149-f03a98747a52)

- 제공자는 자신의 상품에 대해품절, 판매 종료와 같은 고유 상태 변경이 가능하다.
- 관리자는 상품에 대해 판매불가로 변경할 수 있으며 판매 가능(판매중)으로 변경 가능한 고유의 권한을 가지고 있다.
- 제공자와 관리자는 각자의 고유한 권한으로 균형있는 상품관리시스템을 구현했다.

**5. 예약/배송/반납 관리(은미)**<br/>

**6. 리뷰 관리(규남)**<br/>

**7. 문의 관리(규남)**<br/>

**8. 정산 관리(은미)**<br/>
![제공자정산](https://github.com/user-attachments/assets/7ceeb1c1-c45b-43cc-ad83-b4d7fd0bdcfe)

- 월별 선택 가능
- 선택한 달의 총 정산금
- 상품별 정산 금액
- 상세 정산 내역

### <관리자>
**1. 메인(예진 & 은미)**<br/>

**2. 회원 관리(사용자, 제공자, 탈퇴자)(규남)** <br/>

**3. 제품 관리(예진)**<br/>

**4. 예약 현황(은미)**<br/>

**5. 매출 현황(은미)**<br/>
![관리자매출](https://github.com/user-attachments/assets/32304d93-135d-436e-98eb-d7823b0a6d40)

- 월별 선택 가능
- 상품별 총 매출 
- 회사별 총 매출

**6.✅챗봇 관리(예진)✅**<br/>
![modifychatbot](https://github.com/user-attachments/assets/cb7b241d-9e03-4fab-bbf5-d8c31d482c9c)

- 관리자는 챗봇 질문 내용을 수정 또는 추가 가능하며 하위 연결 질문 여부, 관리자 연결 여부를 조절 가능
- 2,3단계에서의 상위 질문은 하위질문여부가 선택 된것만 출력

**7.✅1:1 문의 답변(예진)✅**<br/>

**8. 공지사항(예진)**<br/>

<br/>







## ✨ 물리 데이터 모델
![물리](https://github.com/user-attachments/assets/2eb97a27-ca81-40df-8b08-e1547827d44f)



## 💡 WIKI

### 📙 Back end

  - 😊[](https://github.com/)


 ### 📘 Front end
  - 😊[](https://github.com/)



<br/>
<br/>
