# Portfolio

안녕하세요! 데이터 분석 및 AI/ML 프로젝트 포트폴리오 리포지토리입니다.
각 폴더는 프로젝트별 상세 보고서, 발표 자료, 사업 계획서 등을 포함하고 있습니다.

---

## 🚀 Projects

### 01. 영화 개봉 전 IMDb 점수 예측 프로젝트 (Project Final Report)

* [cite_start]**프로젝트 개요:** 영화 개봉 전, 장르, 상영 시간, 감독, 배우 등의 정보를 활용하여 IMDb 점수를 예측하는 머신러닝 모델을 개발했습니다[cite: 1082].
* [cite_start]**데이터:** IMDb 비상업용 데이터셋(title.basics, title.crew 등)을 다운받아 전처리 및 피처 엔지니어링을 수행했습니다[cite: 1088, 1090, 1091, 1092, 1093, 1094].
* [cite_start]**모델링:** Logistic Regression, RandomForest, AdaBoost, Bagging, GradientBoosting, **XGBClassifier** 등 6가지 모델의 성능을 비교했습니다[cite: 1195].
* **주요 성과:**
    * [cite_start]GridSearchCV를 활용하여 하이퍼파라미터 튜닝을 진행했습니다[cite: 1196].
    * [cite_start]**XGBClassifier** 모델이 67%의 정확도로 가장 좋은 성능을 보였습니다[cite: 1218, 1219].
    * [cite_start]데이터 특성 간의 낮은 상관관계와 'Hit Movie'/'Flop Movie' 간의 불분명한 특성 차이가 정확도에 영향을 미쳤음을 분석했습니다[cite: 1222, 1223].

### 02. 성남시 스쿨존 내 사고분석 및 예방 (2023)

* [cite_start]**프로젝트 개요:** 성남시 스쿨존의 안전시설물(옐로우 카펫, 방호 울타리, CCTV 등) 데이터가 실제 교통사고 발생 유무에 미치는 영향을 분석하고 사고를 예측하는 아이디어 제안서입니다[cite: 7, 8, 9].
* [cite_start]**데이터:** 성남시 및 인근 4개 시(수원, 하남, 광명, 구리)의 스쿨존 데이터를 학습 및 테스트에 사용했습니다[cite: 9].
* [cite_start]**모델링:** StratifiedK-Fold 및 GridSearchCV를 사용하여 Logistic Regression, RandomForest, SVM, **AdaBoost** 모델의 성능을 비교했습니다[cite: 11, 95, 96].
* **주요 성과:**
    * [cite_start]**AdaBoost** 모델이 가장 높은 정확도와 F1-score를 보여 최종 모델로 채택되었습니다[cite: 11, 142].
    * [cite_start]분석 결과, '옐로우 카펫 존 유무'와 '울타리 길이'가 사고 예방에 큰 영향을 미치는 핵심 요인임을 발견했습니다[cite: 12].
    * [cite_start]가설과 달리 '과속방지턱'과 '안전표지판'은 사고 예방에 미미한 영향을 끼쳤으며, 이는 설치 의무 목적의 형식적인 설치 때문일 수 있다고 분석했습니다[cite: 14, 15].
    * [cite_start]성남시 3개 구 중 분당구(특히 서현동, 정자동, 야탑동)에 사고 위험 스쿨존이 가장 많음을 시각화 자료와 함께 제시했습니다[cite: 18, 19, 182].

### 04. 캡스톤 프로젝트_장려상(2024) - 자연어 처리(NLP)를 이용한 인천대 챗봇 '인챗'

* [cite_start]**프로젝트 개요:** 인천대 재학생과 유학생을 위한 자연어 처리(NLP) 기반 챗봇 '인챗(INChat)' 애플리케이션 개발 프로젝트입니다[cite: 201, 221, 222].
* [cite_start]**핵심 기능:** 정해진 시나리오 기반이 아닌, 학교 홈페이지의 PDF 문서를 실시간으로 검색하여 GPT 모델이 답변을 생성하는 RAG(Retrieval-Augmented Generation) 방식을 구현했습니다[cite: 223, 224, 225].
* **개발 스택:**
    * [cite_start]**AI/Model:** `gpt-3.5-turbo`, `LangChain`, `OpenAI Embeddings`, `FAISS` (Vector Store)[cite: 246, 251, 252, 492, 494, 497].
    * [cite_start]**Back-end:** `Python`, `Flask`, `AWS`[cite: 246, 248, 249].
    * [cite_start]**Front-end:** `Android Studio`, `Java`[cite: 243, 247].
* **주요 성과:**
    * [cite_start]`LangChain Auto-Evaluator`를 사용해 영어/한국어 환경에서 GPT 버전별(gpt-3.5 vs gpt-4), Retriever 방식별(TF-IDF vs similarity-search) 성능을 비교 평가했습니다[cite: 255, 269, 364].
    * [cite_start]한국어 평가 시 Auto-Evaluator의 한계(영어로 QnA 생성)를 파악하고, 직접 제작한 QnA 세트로 성능을 재평가하여 Retrieval Score 85점, Answer Score 83점을 달성했습니다[cite: 462, 478, 481, 483].
    * **2024년 캡스톤 프로젝트 장려상**을 수상했습니다.

### 05. ICT SW 여성 창업공모전 (2024) - '돌고돌아'

* [cite_start]**프로젝트 개요:** 기후 위기로 인한 농산물 가격 변동 및 유통비 문제를 해결하기 위한 '돌고돌아' 앱 서비스 사업계획서입니다[cite: 665, 667, 705].
* [cite_start]**핵심 아이템:** 날씨, 유통, 농가 정보 등 **공공데이터를 활용한 농산물 직송 거래 AI 앱**입니다[cite: 704].
* **비즈니스 모델:**
    * [cite_start]AI가 공공데이터(기상청, 농림축산식품부 등)와 농가 정보를 분석하여 수요자(소비자)의 취향에 맞는 농산물을 큐레이션하고 농가와 매칭합니다[cite: 719, 738, 776, 781].
    * [cite_start]농가는 안정적인 수요망을 확보하고, 소비자는 유통 단계를 최적화하여 합리적인 가격으로 농산물을 구매할 수 있습니다[cite: 716, 720].
* **주요 성과:**
    * [cite_start]2024년 ICT/SW 여성 창업공모전에 제출한 비즈니스 모델입니다[cite: 646].
    * [cite_start]시장 분석(온라인 농산물 거래 시장 약 8조원 규모) [cite: 812, 816, 819, 836][cite_start], 경쟁사 분석(마켓컬리, 푸드뱅크), 명확한 자금 조달 및 사업화 계획을 수립했습니다[cite: 850, 883, 924].
