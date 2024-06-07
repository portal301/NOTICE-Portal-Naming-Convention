# Portal301 Project Repository Namaing convention
[Portal 301 프로젝트 명명 규칙](https://github.com/portal301/NOTICE-Portal-Project-Conventions/blob/main/Portal301%20Project%20Repository%20Namaing%20convention)
<br>

# Project Code/Git Behavior Convention

## Objective
브랜치 관리와 컨벤션 통일을 통한 협업 방식은 팀 협업을 위한 중요한 규칙이지만, 모든 프로젝트에서 이를 100% 동일하게 적용할 필요는 없습니다. 각 프로젝트는 고유한 요구사항과 상황을 가지고 있으며, 이러한 규칙은 프로젝트의 특성과 팀의 필요에 따라 유연하게 조정될 수 있습니다.

따라서, 아래에 명시된 Code/Git Behavior Convention은 프로젝트의 참여자들 간의 합의를 통해 변경될 수 있습니다. 프로젝트 팀은 협의를 통해 최적의 방식을 찾아나갈 수 있으며, 이를 통해 프로젝트의 효율성과 효과성을 극대화할 수 있습니다. 예를 들어, 일부 프로젝트에서는 특정 브랜치 정책이 더 효과적일 수 있으며, 다른 프로젝트에서는 보다 간단한 코드리뷰 절차가 적합할 수 있습니다.

결론적으로, 이 문서는 협업을 위한 가장 기본적인 형태의 작업 약속을 지정해둔 문서입니다. 이 문서는 프로젝트 팀이 효율적이고 원활하게 협력할 수 있는 기본 틀을 제공하며, 이를 통해 프로젝트의 성공적인 수행을 지원하고자 합니다.

## Code Convention
[Portal 301 코드 컨벤션](https://github.com/portal301/NOTICE-Portal-Project-Conventions/blob/main/Code%20Convention.md)

## Git Behavior Convention
[Portal 301 Git 사용 규칙](https://github.com/portal301/NOTICE-Portal-Project-Conventions/new/main)

### Pull Request 가이드라인
#### 개요
Pull Request는 협업 개발 환경에서 코드 변경 사항을 제안하고 리뷰하는 중요한 도구입니다. 개발자가 새로운 기능을 추가하거나 버그를 수정한 후, 자신의 브랜치에서 작업을 완료하면, Pull Request를 통해 변경 사항을 메인 브랜치에 병합할 것을 요청합니다. 이 과정에서 팀원들은 제안된 변경 사항을 검토하고, 코드의 품질을 보장하며, 잠재적인 문제를 발견할 수 있습니다. 코드 리뷰어들은 피드백을 제공하고, 필요한 경우 추가 수정 사항을 요청합니다. 이러한 절차를 통해 코드의 안정성과 일관성을 유지하고, 협업 개발의 효율성을 높일 수 있습니다.
#### 사용 방법
- Pull Request의 작업 단위는 빌드 파일의 변화를 제외하고 ***+500/-500***을 넘지 않는것이 이상적입니다.
- 너무 많은 양의 코드 리뷰 요청은 리뷰어가 이해하기 힘들뿐더러, 리뷰의 질적 하락을 야기할 수 있습니다.

##### 등록
1. Branch의 Feature 작업이 완료되면, 작업 Repo 페이지에 접속하여 상단의 Pull Request를 클릭합니다.
   ![image](https://github.com/portal301/NOTICE-Portal-Naming-Convention/assets/5483768/1078cfb9-7b95-4576-b398-176cd77662c1)
2. 병합될 브랜치를 ```Comparing Branch```로 설정하고, 병합의 목적지가 될 브랜치를 ```Base Branch```에 설정합니다. 이후 ```Create Pull Request``` 버튼을 클릭합니다.
   ![image](https://github.com/portal301/NOTICE-Portal-Naming-Convention/assets/5483768/2201570b-9095-4c97-bfba-b3a181ee274f)
3. 제목에 간략한 Feature의 목적을 작성후(1)
4. ```Reviewer```에 코드 리뷰를 해줄 담당자를 등록합니다.(2)
5. ```Assignee```에는 해당 브랜치에 작업을 한 사람을 지정합니다.(3)
6. 이후 작업 내용에 대해 적습니다.(4)  
   ![image](https://github.com/portal301/NOTICE-Portal-Naming-Convention/assets/5483768/3b50085b-adf0-407e-87e2-3941e9f359b6)
7. Create Pull Request 버튼을 눌러 PR을 등록합니다.

##### 리뷰
1. 리뷰어는 코드리뷰를 요청받으면, 전체 파일을 훑어봅니다.
2. 이때 확인이 완료된 코드는 ```viewed``` 버튼을 클릭해 지워나갑니다.
   ![image](https://github.com/portal301/NOTICE-Portal-Naming-Convention/assets/5483768/4ddb5209-beef-4724-a172-fe0bef18969f)
3. 코드상에 문제나 궁금함이 있으면, 각 라인 앞에 마우스를 올려놓으면 생기는 ```+``` 버튼을 눌러 코맨트를 남길 수 있습니다.
   ![image](https://github.com/portal301/NOTICE-Portal-Naming-Convention/assets/5483768/f0ff4126-f8b1-477f-9676-f3436842f84b)
4. 전체 파일이 완료되었다면 ```Review Changes``` 버튼을 눌러 코멘트를 남기거나, 해당 PR의 Merge를 ```Approve``` 할 수 있습니다.
   ![image](https://github.com/portal301/NOTICE-Portal-Naming-Convention/assets/5483768/71676101-6a1a-4c9a-8b79-e6055f0fa9bd)

##### Merge
1. 리뷰가 완료된 PR은 ```Merge Pull Request``` 버튼을 눌러 ```base branch```로 병합할 수 있습니다.
![image](https://github.com/portal301/NOTICE-Portal-Naming-Convention/assets/5483768/67cb0c86-5953-4cad-8a5b-86a20e5b69fa)
2. 이 과정에서 ```Squash and Merge```를 권장하며, 원격 repo에 존재하는 ```compare``` 브랜치는 버튼을 통해 삭제합니다.

#### 템플릿
1. 원격 Repository 디렉토리 최상단에 ```.github``` 폴더를 생성합니다.
2. ```.github```폴더 안에 ```PULL_REQUEST_TEMPLATE.md```파일을 생성 후 아래의 템플릿을 복사 & 붙여넣기 합니다.

```
## 🧑‍💻 PR 내용

 - 수정/추가한 내용을 적어주세요.
 - 수정/추가한 내용을 적어주세요.
 - 수정/추가한 내용을 적어주세요.
```
<hr>

### Git commit log 간지나게 보는법
1. 커맨드 라인 툴에서 ```nano ~./gitconfig```를 입력합니다. 다른 텍스트 편집기로 ```~./gitconfig```를 수정하셔도 됩니다.
2. 다음 내용을 복사 후 붙여넣기 합니다.
	 ```
	[alias]
	lg1 = log --graph --abbrev-commit --decorate --format=format:'%C(bold blue)%h%C(reset) - %C(bold green)(%ar)%C(reset) %C(white)%s%C(reset) %C(dim white)- %an%C(reset)%C(auto)%d%C(reset)' --all
	lg2 = log --graph --abbrev-commit --decorate --format=format:'%C(bold blue)%h%C(reset) - %C(bold cyan)%aD%C(reset) %C(bold green)(%ar)%C(reset)%C(auto)%d%C(reset)%n''          %C(white)%s%C(reset) %C(dim white)- %an%C(reset)'
	lg = lg1
	```
3. 윈도우 기준 ```ctrl + x```를 눌러 저장합니다.
4. 프로젝트 폴더로 이동해 ```git lg```를 입력합니다.
5. 짜잔
   ![image](https://github.com/portal301/NOTICE-Portal-Naming-Convention/assets/5483768/a1056634-fb24-462f-91bb-908e454ff655)
