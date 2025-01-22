# ypl-BE

# 🔗Link

---

BE - API 개발 

[Bitbucket](https://bitbucket.org/youth-policy-list/ypl-be)

BE - 스케줄러 개발

[Bitbucket](https://bitbucket.org/youth-policy-list/ypl-scheduler/src/main/)

App Store

[‎청정리 - 청년 정책 리스트](https://apps.apple.com/kr/app/%EC%B2%AD%EC%A0%95%EB%A6%AC-%EC%B2%AD%EB%85%84-%EC%A0%95%EC%B1%85-%EB%A6%AC%EC%8A%A4%ED%8A%B8/id6448850043)

# 🗨️소개
## 📱프로젝트 소개

[Simulator Screen Recording - iPhone 14 Pro - 2023-01-31 at 23.41.01.mp4](https://prod-files-secure.s3.us-west-2.amazonaws.com/02fe32fb-a454-4c7f-89fd-4e823a1f27bf/755575c2-0356-4e06-a44f-96612b4a30ed/Simulator_Screen_Recording_-_iPhone_14_Pro_-_2023-01-31_at_23.41.01.mp4)

<aside>
<img src="/icons/info-alternate_blue.svg" alt="/icons/info-alternate_blue.svg" width="40px" /> 청정리 앱은 현재 신청 가능한 정책을 확인할 수 있는 앱입니다.

</aside>

<aside>
<img src="/icons/search_blue.svg" alt="/icons/search_blue.svg" width="40px" /> 키워드, 정책 카테고리, 지역, 연령, 취업상태
총 5가지의 검색 조건으로
나에게 맞는 정책을 검색할 수 있습니다!

</aside>

<aside>
<img src="/icons/send_blue.svg" alt="/icons/send_blue.svg" width="40px" /> 현재 보고 있는 정책 공유도 가능합니다.

</aside>

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/02fe32fb-a454-4c7f-89fd-4e823a1f27bf/99c1b087-0db7-4b3f-ae90-8e4d7ea1a9de/Untitled.png)


# 🛠️개발 스택

---

### 개발 환경

- IDE : IntelliJ
- 언어 : Java 11
- 프레임워크 : Spring Boot
- 라이브러리 : JPA
- 빌드 도구 : Gradle
- 데이터 베이스 : AWS RDS(Maria DB)
- Etc : Git, [ERD Cloud](https://www.erdcloud.com/d/MKfb7iST695yfcJ5Z)

### 협업 툴

- API 문서화 : Swagger, [Gitbook](https://undefined-475.gitbook.io/ypi-api-docs/reference/ypl-api/main)
- 이슈 트래커 : JIRA
- 문서 관리 : Notion
- 커뮤니케이션 : Discord

  ## 프로젝트 구조

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/02fe32fb-a454-4c7f-89fd-4e823a1f27bf/e9fc5cb2-4f77-4d86-8933-414d2a571a0f/Untitled.png)

## ERD 설계

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/f73d153e-b42e-48a0-9ac2-ffbda59c20b2/Untitled.png)


## 앱 구조

[Screen Recording 2023-02-01 at 0.13.36.mov](https://prod-files-secure.s3.us-west-2.amazonaws.com/02fe32fb-a454-4c7f-89fd-4e823a1f27bf/dfea34fb-84c6-4127-b579-aabd0db77168/Screen_Recording_2023-02-01_at_0.13.36.mov)

### 1. 메인 화면

- 메인 화면 상단에는 정책 카테고리별로 **조회수가 가장 높은** 정책을 보여주며 **하루 단위**로 갱신됩니다. (6개)
    - Scheduler를 이용하여 1일 단위 API 조회하여 정책을 DB에 저장 및 업데이트 해주었습니다.
    - 조회 수 기준 정책 조회 API를 제공하였습니다.
- 아래 카테고리 버튼은 터치하면 해당 카테고리 필터가 선택된 [검색 화면](https://www.notion.so/33b17bdb108f454ea27c0af9ef64ce42?pvs=21)으로 이동합니다.
- 카테고리 버튼 아래 이미지도 검색 화면으로 이동하는 버튼입니다.
- 노션 이미지는 YPL 팀 소개 페이지로 이동하는 버튼입니다.

[Screen Recording 2023-02-01 at 0.19.01.mov](https://prod-files-secure.s3.us-west-2.amazonaws.com/02fe32fb-a454-4c7f-89fd-4e823a1f27bf/eb515be7-6b57-4ad1-aa84-7763637c57e0/Screen_Recording_2023-02-01_at_0.19.01.mov)

### 2. 정책 상세 화면

- 정책 상세 화면에는 **정책 상세, 신청 자격, 신청 방법** 섹션으로 구분되어 있습니다.
    - 정책 세부 내용 API를 제공하였습니다.
- 정책 상세 섹션 우측 **공유**하기 버튼을 터치하면 현재 정책의 축약된 정보를 공유할 수 있습니다.

### 3. 검색 화면

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/02fe32fb-a454-4c7f-89fd-4e823a1f27bf/5c962ef3-4abe-4c33-a4ed-6012b1035fe0/Untitled.png)

[Screen Recording 2023-02-01 at 0.28.18.mov](https://prod-files-secure.s3.us-west-2.amazonaws.com/02fe32fb-a454-4c7f-89fd-4e823a1f27bf/296f5e79-0bb5-455f-9659-d7f6b61f6af8/Screen_Recording_2023-02-01_at_0.28.18.mov)

- 검색 화면은 [메인 화면](https://www.notion.so/33b17bdb108f454ea27c0af9ef64ce42?pvs=21)에서 4가지 종류의 버튼을 터치하여 이동할 수 있습니다.
- 상단에 있는 검색 텍스트필드를 이용하여 **키워드 검색**이 가능합니다.
    - 필터 적용하여 데이터 조회 하는 API를 제공하였습니다.
    - 카테고리별 데이터 조회 API를 제공하였습니다.
- 검색 필터는 접었다 펼 수 있습니다.
- 연령 조건은 **최소, 최대** 나이를 지정할 수 있으며 해당 범위에 속한 정책만 검색됩니다.
- 검색하기 버튼을 터치하면 **현재 선택된 조건**에 따라 결과를 보여줍니다.
- 검색 결과는 한번에 **최대 12개**씩 불러오며, 아래로 스크롤하여 더 불러올 수 있습니다.
- 우측에는 새로고침 버튼으로 같은 조건을 **재검색**해서 결과를 가져옵니다.
