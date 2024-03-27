# sesac_team_project_dl

[SeSAC x Saltlux]LLM 활용 인공지능 서비스 개발자 양성과정에서 진행한 mini-project<br />

### 프로젝트 소개

---

<strong>[주제 : 뉴스 기사 자동 분류]</strong><br />

- 세부 내용 : 뉴스 기사를 입력으로 넣어주면 정치, 경제, 사회, 국제 4가지의 column중에서 기사가 해당하는 컬럼이 무엇인지 알고 모델별 성능 비교와 확인<br />
- 작업 기간 : 2024.03.22 ~ 2024.03.27 <br />

<strong>[프로젝트 목적]</strong><br />

- 기본적인 NLP에 대한 내용을 학습 후 학습한 내용의 실습
- Text classification을 할 수 있는 모델 파이프라인을 구축 후 성능 비교 및 평가

### 절차 및 결과

---

<strong>[데이터 크롤링 및 전처리]</strong><br />

- 중앙일보, 동아일보, 한겨레, 한국일보 23년 분기별 - 정치, 경제, 사회, 국제 4가지 column에 대해 150개씩 추출
- 이메일 주소, url, 이모티콘, 한자, 특수문자, 괄호, 일본어 등 제거

<strong>[모델 개발 및 성능 비교]</strong><br />

- KoBERT(https://github.com/SKTBrain/KoBERT?tab=readme-ov-file)
- Roberta(https://huggingface.co/FacebookAI/xlm-roberta-base)
- KoELECTRA(https://huggingface.co/Copycats/koelectra-base-v3-generalized-sentiment-analysis)
- BERT(https://huggingface.co/google-bert/bert-base-multilingual-cased)

| Model     | Accuracy |
| --------- | -------- |
| KoBERT    | 94.17%   |
| Roberta   | 77.08%   |
| KoELECTRA | 91.66%   |
| BERT      | 90.28%   |

<strong>[Gradio를 통한 확인]</strong>
![image](https://github.com/seojunho97/sesac_team_project_dl/assets/106465767/22d9fa64-8137-4d6c-b75f-6bca2eae00de)
### 팀원 소개

---

- 서준호<br />
- 정승용<br />
- 홍성균<br />
- 김도현<br />
