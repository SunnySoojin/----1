# 주의사항: main이나 master 브랜치 이름은 사용자의 깃 설정에 따라 다를 수 있습니다. 이 예제에서는 master 브랜치를 사용합니다. 만약 작동을 안할경우 main을 사용해주세요.
# 새로운 깃 저장소 초기화
git init
# 지금 있는 브랜치 확인(commit이 되어야 나옵니다.)
git branch
# 파일 하나 a.txt 생성합니다. 생성한 후 아래 명령어를 쳐주세요.
# 내가 현재 수정한 파일을 관리하는 곳에 추가
git add .
# 버전을 추가
git commit -m "첫 커밋"
# 지금 있는 브랜치 확인
git branch
# 파일 하나 더 추가해보겠습니다. b.txt 생성 후 아래 명령어를 쳐주세요.
git add .
git commit -m "두 번째 커밋"
# 지금 있는 브랜치 확인
git branch
# 새로운 a, b 브랜치 생성
git branch a
git branch b
# 브랜치 확인
git branch
# a 브랜치로 이동
git checkout a
# 브랜치 확인
git branch
# a 브랜치에서 파일 aa.txt 생성 후 아래 명령어를 쳐주세요.
git add .
git commit -m "a 브랜치"
# 브랜치 이동
git checkout b
git branch
# b 브랜치에서 파일 bb.txt 생성 후 아래 명령어를 쳐주세요.
git add .
git commit -m "b 브랜치"
# 브랜치 이동(master는 main일 수도 있습니다. 여러분 브랜치 확인해주세요.)
git checkout master
git branch
# 브랜치 병합
git merge a
git merge b
# 병합 메시지 발생되면 메시지 입력후 저장 후 종료