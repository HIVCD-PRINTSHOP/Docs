<div align="center">
  <h1 align="center" style="line-height: 50px;">HIVCD PRINTSHOP <br/>TEAM DEVELOP PROGRESS</h1>
    <h3  align="center">우리가 <span style="color: #75c375">Github Project</span>를 활용하여 프로젝트 관리하는 법</h3>
    <a href="#-git-flow">Git Flow</a>
    &middot;
    <a href="#-commit-규칙">Commit 규칙</a>
    &middot;
    <a href="#-issue--pr">Issue & PR</a>
</div>

<br/>
<br/>
<br/>

### 🪵 Git Flow
Git Flow는 소프트웨어 개발에서 브랜치를 체계적으로 관리하는 방법론으로, 팀 협업을 극대화하고 코드 품질을 향상시키는 데 중점을 둡니다. 명확한 브랜치 구조를 통해 개발, 테스트, 배포 단계를 구분하고, 개발자들이 독립적으로 작업할 수 있도록 지원합니다. 기능 개발, 버그 수정, 배포 준비를 위한 다양한 브랜치를 정의하여 프로젝트의 복잡성을 줄이고 가시성을 높입니다.


![images_kw2577_post_9f1340a8-80f7-4c6a-ada5-d93ab0d877c9_image](https://github.com/user-attachments/assets/21a47425-19ed-4ba6-bd17-7e92cd833fe9)

Git flow 방법론을 활용하기 위해, Team Develop에서 정의한 주요 Branch의 역할은 다음과 같습니다.

✔️ **main (master)**
이 브랜치는 기준이 되는 브랜치로, 최종 제품이 배포되는 곳입니다.

✔️ **develop**
개발 브랜치로, 개발자들이 각자 작업한 기능을 해당 브랜치에 merge하여 통합합니다.

✔️ **feature**
단위 기능을 개발하기 위한 브랜치이며, 기능 개발이 완료되면 해당 브랜치는 PR을 통해 develop 브랜치에 merge됩니다. 
> 📍 **Feature Branch 이름 규칙**
> 
> - 이슈 번호를 포함하여 명시합니다. 
> - 양식 : feature/{issue-number}-{feature-name}
>   *Ex. feature/12-add-login-api*

✔️ **release**
배포를 위해 master 브랜치로 보내기 전, 품질 검사를 위한 QA를 수행하는 브랜치입니다. 
> 📍 **Release Branch 이름 규칙**
> 
> - 배포 날짜 기반으로 작성합니다.
> - 양식 : release/배포날짜(YYMMDD)
>   *Ex. release/250224*

✔️ **hotfix**
master 브랜치에 배포 후 발생한 버그를 긴급하게 수정하기 위한 브랜치입니다.
> 📍 **Hotfix Branch 이름 규칙**
> 
> - 버그가 발생한 기능을 기반으로 작성합니다.
> - 양식 : **hotfix/버그 발생 지점**
>   *Ex. hotfix/login-error*

<br/>
<br/>


### 📬 Commit 규칙
팀 Develop에서는 일관된 commit 메시지를 사용하여 프로젝트의 변경 이력을 명확하게 기록하고 있습니다. 이를 위해 자체 commit 규칙을 마련하였습니다.


**✔️ 기본 사항**
- 모든 내용은 영어로 작성합니다.
- 제목과 본문은 빈 행으로 구분합니다.

1️⃣ **제목**
- 제목은 50자 이내로 작성하며, 첫 글자는 대문자로 시작해야 합니다.
- 제목 끝에 마침표를 사용하지 않으며, branch 생성한 이슈 번호를 작성합니다.

2️⃣ **본문**
변경한 내용과 그 이유를 설명해야 하며, "어떻게" 보다는 "무엇"과 "왜"에 중점을 두어 작성합니다.

3️⃣ **유형**
Commit 유형에 따라, 제목에 다음과 같은 접두사를 사용합니다.
| Commit 유형  |  상세 설명  |
|:---:|:---:|
| FEAT   |  새로운 기능 추가  |
| ADD   |  간단한 코드나 문서 추가  |
| REMOVE   |  코드나 문서 삭제  |
| FIX   |  버그 수정 |
| DOCS   |  문서 수정 |
| REFACTOR   |  코드 리팩토링 |
| TEST   |  테스트 코드 추가 또는 리팩토링 |
| CHORE   |  빌드 작업 수정이나 패키지 매니저 수정 (예: .gitignore 수정)  |
| INIT   |  초기 설정  |

<br/>

👍 **예시**
- Feat: add support for ETag option in res.sendFile (#10)
- Docs: add documentation for new API endpoints (#32)

<br/>
<br/>

### 🔁 Issue & PR 시스템
팀 Develop에서는 GitHub의 Label 설정과 Issue 템플릿을 도입하여 이슈 관리와 기능 요청을 효율적으로 진행하고 있습니다.


✔️ **Label 속성**
| Label 이름  |  상세 설명  |
|:---:|:---:|
| 🐞 BugFix   |  버그 수정  |
| 🌏 Deploy   |  배포 관련  |
| ✨ Feature   | 기능 개발  |
| ⚙ Setting   |  개발 환경 세팅 |
| 🎨 Style   |  마크업 & 스타일링 |
| ✅ Test   |  test 관련 |
| 📬 API   |  서버 API 통신 |
| 🧹 cleanup   |  코드를 더 깔끔하게 만들기만 하고, 코드 작동 방식이나 출력에 대한 부분을 변경 X  |
| 💻 CrossBrowsing   |  브라우저 호환성  |
| 📃 Docs   |  문서 작성 및 수정  |
| 🔨 Refactor   |  코드가 내부적으로 작동하는 방식을 변경  |
| 참여 개발자 이름  |  해당 이슈를 담당하는 개발자를 지정  |

<br/>
<br/>

✔️ **Issue Template**
> **Feature Request 양식**
> 새로운 기능을 구현할 때 사용합니다.
> 
> ![image](https://github.com/user-attachments/assets/cdbf7f14-a115-4f1b-8580-02bebfc865d7)

> **Bug Report 양식**
> 버그가 발생해서 수정이 필요할 때 사용합니다.
> 
> ![image](https://github.com/user-attachments/assets/a7b8fa40-9d28-457a-af44-cb061e23c839)

