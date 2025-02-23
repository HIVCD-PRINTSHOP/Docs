<div align="center">
  <h1 align="center" style="line-height: 50px;">HIVCD PRINTSHOP <br/>TEAM DEVELOP PROGRESS</h1>
    <h3  align="center">우리가 <span style="color: #75c375">Github Project</span>를 활용하여 프로젝트 관리하는 법</h3>
    <a href="#-github-project란">Github Project란?</a>
    &middot;
    <a href="#️-자체-개발-프로세스">자체 개발 프로세스</a>
    &middot;
    <a href="#-우리-만의-github-project">우리 만의 Github Project</a>
</div>

<br/>
<br/>
<br/>

### 👀 Github Project란?
**GitHub에서 제공하는 프로젝트 관리 툴**로, 소프트웨어 개발을 보다 효율적으로 지원합니다.
이와 유사한 도구로는 Jira, Notion, Trello 등이 있습니다. 

[추후 사진 첨부 예정]

최근 많은 기업들이 프로젝트 관리 툴로 Jira를 선택하여 사용하고 있지만, 저희 팀은 GitHub Project를 선택한 몇 가지 이유가 있습니다.

1️⃣ 저희 개발 팀은 5~6인 소규모로 구성되어 있어 Jira와 같은 복잡한 툴은 적합하지 않았습니다.
2️⃣ 팀원 모두가 GitHub을 필수적으로 사용하고 있기 때문에, 접근성과 사용 편의성이 높은 GitHub Project를 선택했습니다. 
3️⃣ 기능 개발 단계에서 QA 단계로 넘어갈 때, 상위 이슈 별로 확인하고 테스트를 진행하기에 수월하다고 판단했습니다.

<br/>
<br/>

### ⚙️ 자체 개발 프로세스
**Github Project**와 **Issue & PR 시스템**을 최대한 활용하고자, 저희 팀에 최적화된 시스템을 만들어 나갔습니다.

1️⃣ 기능 명세서와 와이어프레임을 분석하여, 주요 기능들을 도출합니다. (By 개발 PM)
2️⃣ 주요 기능 1개를 선정한 뒤, GitHub Project의 Docs Repo에 이슈 형태로 등록하며, 해당 이슈는 상위 이슈로 유지됩니다. (By 개발 PM)
3️⃣ 선택한 기능의 Frontend와 Backend 범위의 기능들로 분리하며, 각각의 Repo에 하위 이슈로 등록합니다. (By, 기능 담당 개발자)
4️⃣ 하위 이슈들이 "In Progress" 단계에 접어들면서 개발 진행합니다.
5️⃣ 기능 구현이 완료되어 Pull Request 요청 시, 관련 분야의 개발자들이 코드 리뷰를 작성하며 피드백을 진행합니다.
6️⃣ 1개의 기능 개발이 완료되었기에, QA 단계로 넘어가서 테스트합니다.

<br/>
<br/>

### 📋 우리 만의 Github Project
Github Project를 처음 도입하다보니, Github에서 제공하는 "**Feature release**" 템플릿으로 최초 세팅했습니다.
![Image](https://github.com/user-attachments/assets/662279ea-a848-47f9-9443-32f78927e4c9)

자체 개발 프로세스에서 설명한 바와 같이, 주요 기능은 **Backlog View**에 이슈 형태로 등록됩니다.

[사진 첨부 예정]

FE와 BE 기능 분류 후 하위 이슈 형태로 등록합니다.

[사진 첨부 예정]

이렇게 이슈들이 등록이 완료되어 개발이 진행되고, 새로운 기능 분류를 시작하게 되면 "**Status Board**"에서 작업들을 관리합니다.

![image](https://github.com/user-attachments/assets/f3a54c0d-2047-4edf-946c-7e9bc9697a3e)

그럼 **Backlog View에 어떤 속성들이 존재**하는 지 궁금하실 분들을 위해 간단하게 정리해봤습니다.

**✔️ Title**
대략적인 기능 요약

**✔️ Status**
| Option  |  상세 설명  |
|:---:|:---:|
| 📃 Backlog   |  제시된 기능 채택 후 정리 단계  |
| 📚 Ready   |  기능에 대한 상세 정보 정리 완료 단계  |
| 🔨 In progress   |  정리된 기능 구현 단계  |
| 👀 In review   |  구현된 기능 검토 단계  |
| ✅ Done   |  기능이 완성되었음을 알리는 단계  |

<br/>

**✔️ Priorty**
해당 Task의 우선 순위
- 🏝️ Low
- 🏕️ Medium
- ⛰️ High
- 🌋 Urgent
<br/>

**✔️ Size**
해당 Task의 예상 난이도
- 🌱 Small
- 🌿 Medium
- ☘️ Large
- 🍀 Extra Large
- 🌴 Giant
<br/>

**✔️ Iteration**
작업 진행할 기간 정의 (1주일 단위)

<br/>
<br/>

<div align="center">
    <h3 align="center">TEAM DEVELOP에서 준비한 글은 여기까지!</h3>
    <h4>끝까지 읽어주셔서 감사합니다.</h4>
    <h6>last updated 2025.02.23</h6>
</div>