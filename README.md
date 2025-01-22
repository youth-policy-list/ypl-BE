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

![image](https://github.com/user-attachments/assets/3e7bf14e-eb1f-439b-8380-213616e5502d)

- 청정리 앱은 현재 신청 가능한 정책을 확인할 수 있는 앱입니다.
- 키워드, 정책 카테고리, 지역, 연령, 취업상태 총 5가지의 검색 조건으로 나에게 맞는 정책을 검색할 수 있습니다!
- 현재 보고 있는 정책 공유도 가능합니다.


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

![image](https://github.com/user-attachments/assets/c6757387-1f8f-4ad0-9431-aefb359684ca)


## ERD 설계

![image](https://github.com/user-attachments/assets/772e41d2-dd07-4617-8493-c82aaeafd2f0)

## 1. 홈 화면

<table>
	<tr>
		<td>
			<img src=https://user-images.githubusercontent.com/31722496/215308311-a8bd7802-a130-4a23-b9ea-250c8698f846.gif width=200>
		</td>
		<td>
			- 홈 화면 상단에는 카테고리별로 조회수가 가장 높은 정책을 보여줍니다. </br>
			- 아래에 있는 정책 카테고리를 선택하면 해당 필터가 선택된 검색 화면으로 이동합니다.
		</td>
	</tr>
</table>



## 2. 상세 화면

<table>
	<tr>
		<td>
			<img src=https://user-images.githubusercontent.com/31722496/215308961-5ee0cc50-6d36-4efc-975f-340ce9b873fe.gif width=200>
		</td>
		<td>
			- 정책의 상세 내용을 확인할 수 있습니다. </br>
			- 공유하기 버튼을 터치하면 정책 정보를 공유할 수 있습니다.
		</td>
	</tr>
</table>


## 3. 검색 화면

<table>
	<tr>
		<td>
			<img src=https://user-images.githubusercontent.com/31722496/215308985-565fffcb-a4e7-4482-af04-290aa8d92709.gif width=200>
		</td>
		<td>
			- 카테고리, 지역, 연령, 취업상태 필터 및 검색어를 통해 정책을 검색할 수 있습니다.
		</td>
	</tr>
</table>


## 4. 팀 소개 화면

<table>
	<tr>
		<td>
			<img src=https://user-images.githubusercontent.com/31722496/215309007-7e559f06-6e69-4e98-8b92-a210f769953c.gif width=200>
		</td>
		<td>
			- 팀 YPL 소개 페이지로 이동합니다. </br>
			- 상단 검색창을 통해 웹 페이지 이동 및 검색이 가능합니다
		</td>
	</tr>
</table>

더 자세한 내용과 개발 이슈는 [Notion 페이지](https://rough-nerve-b7c.notion.site/33b17bdb108f454ea27c0af9ef64ce42?pvs=4)에서 확인하실 수 있습니다.
