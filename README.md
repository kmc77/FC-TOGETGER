# FC-TOGETGER

## 🔐 Repository 비어있는 이유 안내

해당 프로젝트의 레포지토리가 비어 있는 이유는 다음과 같습니다

1. **개발 초기 팀원과 브랜치/메인 구조로 협업하며 커밋된 `application.properties` 파일이 Git 이력에 포함되는 문제가 발생**.
2. 이후 `.gitignore`를  적용하여 해당 파일은 Git 추적에서 제외되었지만 과거 커밋에 이미 포함된 민감 정보가 여전히 남아 있는 상태.
3. `main`브랜치 병합 후 GitHub에 업로드되며 AWS Access Key 노출, AWS 측에서 자동 보안 정책 `AWSCompromisedkeyQuarantinev2` 적용.
4. AWS 측과도 메일을 통해 정책 해제를 요청했으나, GitHub의 캐시 또는 서드파티 백업 시스템으로 인해 키값이 계속 검색에 노출되었음.

