# 작업 규칙 (samkoo-dx 공통)

## 1. 브랜치
- develop에서 분기: `feature/<이슈번호>-<내용>`, `fix/<내용>`
- main 대상 PR: `release/*`, `hotfix/*`만 허용 (solo 레포는 develop도 허용)
- main·develop 직접 push 금지

## 2. 커밋
- 형식: `<유형>: <요약>` (50자 이내, 명사형)
- 유형: feat, fix, docs, refactor, test, chore
- 템플릿 설정(1회): `git config --global commit.template .gitmessage.txt`

## 3. PR
- 이슈 등록 → 브랜치 생성 → PR 작성 순서
- 본문에 `Closes #이슈번호` 기재
- develop 병합: Squash / main 병합: Merge
- team 레포: 동료 1인 승인 / solo 레포: main 병합 시 DX전략팀·보안팀 1인 승인

## 4. 금지 사항
- .env, 키 파일, 토큰 등 비밀정보 커밋 금지
- 업로드 이미지·첨부파일 커밋 금지 (GCP 버킷 사용)
- 개인 레포에서 사내 소스 작업 금지
