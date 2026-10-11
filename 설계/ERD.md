# 주요 데이터 구조 및 ERD 초안

## User

사용자 정보를 관리한다.

```text
user_id
name
email
password_hash
created_at
```

---

## Resume

사용자가 등록한 이력서 정보를 관리한다.

```text
resume_id
user_id
file_url
resume_text
created_at
```

---

## Job

사용자가 지원하려는 기업 및 직무 정보를 관리한다.

```text
job_id
user_id
company_name
job_position
job_description
```

---

## Interview

사용자가 진행한 면접 정보를 관리한다.

```text
interview_id
user_id
resume_id
job_id
score
feedback
created_at
```

---

## Interview Question

면접에서 AI가 생성한 질문을 관리한다.

```text
question_id
interview_id
question
question_type
```

---

## Interview Answer

각 질문에 대한 사용자의 답변을 관리한다.

```text
answer_id
question_id
answer_text
score
feedback
```

---

> 현재 기획서의 데이터 항목을 옮긴 초안입니다. 테이블 관계와 자료형은 ERD 확정 시 추가합니다.
