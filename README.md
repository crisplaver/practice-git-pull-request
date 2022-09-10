# Pull Request 방식

## 원격 저장소에 대한 권한이 있는 경우
- 일반적인 경우 활용 

### Pull Request 과정
1. branch를 생성한다
2. 코드 수정 후 origin에 branch를 푸시한다
3. Github에서 Pull Request를 생성한다
4. Merge 후 코드를 동기화한다
```
git pull
```
## 원격 저장소에 대한 권한이 없는 경우
- 일반적으로 오픈소스에서 활용

### Pull Request 과정
1. 저장소를 fork하고 원본 프로젝트의 원격 저장소를 추가한다
```
git remote add upstream <원본 저장소 주소>
```
2. branch를 생성한다
3. 코드 수정 후 origin에 커밋한 내용을 푸시한다
4. Github에서 Pull Request를 생성한다
5. Merge 후 코드를 동기화하고 브랜치를 삭제한다
```bash
git pull upstream main
git branch -d <branch-name>
```
