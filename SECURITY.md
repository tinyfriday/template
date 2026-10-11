# 보안

## 제보

취약점은 공개 이슈 대신 이 저장소의 **Security → Report a vulnerability** 로 알려 주세요.

## 기본 체크리스트 (PRINCIPLES 5절)

- [ ] CI 통과해야 병합 (린트·테스트·빌드)
- [ ] Dependabot 켜짐, CodeQL 켜짐, 비밀값 검사(secret scanning) 켜짐
- [ ] 비밀값은 GitHub Secrets·환경 변수로만. 저장소에 없음
- [ ] HTTPS, 보안 헤더(CSP). 외부 스크립트는 꼭 필요한 것만 허용
- [ ] BYOK 키는 사용자 기기에만. 서버로 보내지 않음

## 위협 모델 (짧게)

| 무엇이 악용될 수 있나 | 막는 방법 |
| --- | --- |
| {예: 입력 파일로 스크립트 주입} | {예: 출력은 textContent 로만} |
