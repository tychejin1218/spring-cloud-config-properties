## Spring Cloud Config Properties

---

## 목차
* [Properties 폴더 구조](#properties-폴더-구조)
* [Properties 파일 작성](#properties-폴더-작성)

---

### Properties 폴더 구조
* application 명
  * profile 명 - local / dev / qa / prod
    * 예) api1/local/
---

### Properties 파일 작성
* *.properties 파일이 아닌 *.yml 파일로 작성
* 파일명은 application 명-설정 파일명-profile 명으로 작성
  * 예) api1-datasource-local.yml
* 설정 파일명
  * DataSource, JPA, Redis 등 RDS, NoSQL 과 관련된 내용은 datasource 명으로 작성
    * 예) api1-datasource-local.yml
  * 암호화, 외부 API 정보, S3, Sentry 등 환경 설정과 관련된 내용은 environment 명으로 작성
    * 예) api1-environment-local
---
