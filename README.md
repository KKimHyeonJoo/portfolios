# Portfolio

안녕하세요! 데이터 분석 및 AI/ML 프로젝트 포트폴리오 리포지토리입니다.
본 리포지토리는 데이터 수집, 전처리, 모델링, 서비스 기획 및 비즈니스화에 이르는 다양한 프로젝트 경험을 담고 있습니다.

## 🚀 Projects

### 01. 캡스톤 프로젝트: 자연어 처리(NLP)를 이용한 인천대 챗봇 '인챗' (2024)

* **[프로젝트]** 2024년 캡스톤 프로젝트 **(장려상 수상)**
* [cite_start]**[역할]** **팀장** (2인 팀) [cite: 3]
* **[개요]** 인천대학교 재학생 및 유학생을 대상으로, 분산된 학교 정보를 통합 제공하는 AI 챗봇 애플리케이션 '인챗'을 개발했습니다. [cite_start]기존의 시나리오 기반 챗봇과 달리, **학교 홈페이지 PDF 문서를 검색**하여 답변을 생성하는 RAG(Retrieval-Augmented Generation) 방식을 구현했습니다[cite: 20, 24, 25, 443].
* **[문제 정의]**
    * [cite_start]학생들(특히 유학생)이 학교 홈페이지에서 원하는 정보를 찾는 데 불필요한 웹 서핑 시간이 소요됩니다[cite: 13, 14].
    * [cite_start]학과 사무실 등은 특정 시간 이후 문의가 불가능합니다[cite: 16].
* **[기술 스택]**
    * [cite_start]**AI & NLP:** `GPT-3.5-turbo` [cite: 286][cite_start], `LangChain` [cite: 46, 51][cite_start], `OpenAI Embeddings`, `FAISS` (Vector Store)[cite: 294, 297].
    * [cite_start]**Back-end:** `Python`, `Flask`, `AWS`[cite: 46, 47, 48, 49].
    * [cite_start]**Front-end:** `Android Studio`, `Java`[cite: 43, 47].
* [cite_start]**[핵심 RAG 파이프라인]** [cite: 285, 298, 332]
    1.  [cite_start]**문서 처리 (Ingestion):** PDF 문서들을 `Langchain Text Spiltter`로 분할하고 `OpenAI Embeddings`를 통해 벡터화하여 `FAISS` 벡터 스토어에 저장합니다[cite: 294, 296, 297].
    2.  [cite_start]**검색 (Retrieval):** 사용자의 질문이 들어오면, `Similarity Search` 리트리버가 벡터 스토어에서 가장 관련성 높은 문서 조각들을 검색합니다[cite: 291, 293].
    3.  [cite_start]**생성 (Generation):** 검색된 문서 조각들과 원본 질문을 `Prompt`로 결합하여 `GPT-3.5-turbo` (LLM)에게 전달, 최종 답변을 생성합니다[cite: 289, 312].
* **[성능 평가 및 개선]**
    * [cite_start]`LangChain Auto-Evaluator`를 사용해 QnA 세트를 자동 생성하고 모델 성능을 평가했습니다[cite: 55, 56].
    * [cite_start]**모델 비교:** `GPT-3.5-turbo`가 `GPT-4`보다 응답 속도(영어 1.87s vs 7.00s)와 성능(영어 Answer Score 90 vs 90) 모두에서 효율적이거나 대등한 결과를 보여 `GPT-3.5-turbo`를 채택했습니다[cite: 81, 82, 86, 88, 95, 97].
    * [cite_start]**한국어 데이터 한계 극복:** Auto-Evaluator가 한국어 문서로 *영어* QnA를 생성하여 성능 평가가 왜곡되는 문제를 발견했습니다[cite: 262].
    * [cite_start]**개선:** 이를 해결하기 위해 **직접 한국어 QnA 세트를 제작**하여 평가를 진행, 최종적으로 **Retrieval Score 85점**, **Answer Score 83점**을 달성했습니다[cite: 278, 281, 283].

---

### 02. ICT/SW 여성 창업공모전: AI 기반 농산물 직거래 앱 '돌고돌아' (2024)

* [cite_start]**[프로젝트]** 2024 ICT/SW 여성 창업공모전 사업계획서 [cite: 446]
* [cite_start]**[역할]** **CEO (대표)** / 컴퓨터공학부 [cite: 545]
* [cite_start]**[개요]** '날씨·유통 공공데이터를 활용한 농가 생산물 직송 거래 AI 앱'이라는 아이템으로, 기후 변화와 복잡한 유통 구조로 인한 농산물 가격 불안정 문제를 해결하고자 했습니다[cite: 504].
* **[문제 정의]**
    * [cite_start]**소비자:** 기후 변화로 인한 생산량 변동으로 농산물 가격 부담이 증가합니다[cite: 495].
    * [cite_start]**생산자:** 유통 비용이 과다(예: 딸기 46.3% [cite: 463, 464][cite_start])하고, 디지털 전환에 어려움을 겪어[cite: 502] [cite_start]안정적인 소득 확보가 어렵습니다[cite: 496].
* **[솔루션]**
    * [cite_start]**AI 데이터 분석:** 기상청 [cite: 562][cite_start], 농림축산식품부 [cite: 576] 등의 **공공데이터**와 농가 생산 정보를 AI로 분석합니다.
    * [cite_start]**수요-공급 매칭:** AI가 생산량을 예측하고, 소비자의 취향(예: 베지테리언, 식습관)에 맞춰 농산물 패키지를 큐레이션하여[cite: 582] [cite_start]생산자와 소비자를 직접 연결합니다[cite: 515, 519].
    * [cite_start]**기대 효과:** 농가는 안정적인 수요망을 확보하고[cite: 520][cite_start], 소비자는 유통 구조 최적화를 통해 합리적인 가격에 고품질 농산물을 제공받습니다[cite: 516, 583].
* [cite_start]**[비즈니스 모델]** [cite: 873]
    * [cite_start]**주요 고객:** 단체 급식 업체, 외식 사업자, 프랜차이즈 (B2B/B2G) [cite: 780, 873] 및 일반 소비자 (B2C).
    * [cite_start]**핵심 가치:** 버려지는 농산물 최소화, 농가 소득 증대, 착한 가격으로 사회적 약자에 제공[cite: 873].
    * [cite_start]**수익원:** 수요자(B2B) 대상 구독 서비스, 생산자 대상 유통 대행 수수료[cite: 873].
    * [cite_start]**시장 규모:** 약 8조 원(2022년 기준 7조 9816억)의 농축수산물 온라인 거래 시장을 타겟으로 합니다[cite: 612, 619, 640].

---

### 03. 데이터 분석 프로젝트: 성남시 스쿨존 내 교통사고 발생 유무 예측 (2023)

* [cite_start]**[프로젝트]** 스쿨존 내 안전시설물 데이터 기반 교통사고 발생 위험 예측 모델링[cite: 1107, 1109].
* [cite_start]**[개요]** 성남시 스쿨존의 사고 예방을 위해, 주변 4개 시(수원, 하남, 광명, 구리)의 데이터를 학습하여 성남시 스쿨존의 사고 위험 유무를 예측하는 모델을 개발했습니다[cite: 1109, 1172].
* **[데이터 전처리 및 피처 엔지니어링]**
    * [cite_start]공공데이터 포털의 원본 데이터를(좌표계 'EPSG:4326'로 변환 [cite: 1168][cite_start]) 스쿨존 중앙 좌표 기준 300m 이내로 필터링했습니다[cite: 1169].
    * [cite_start]`haversine` 라이브러리로 거리를 계산하여 '횡단보도 개수', '안전표시판 개수', '과속방지턱 개수' 등의 피처를 생성했습니다[cite: 1169, 1170].
    * [cite_start]`StandardScaler`로 데이터 스케일링을 진행했습니다[cite: 1186].
* **[모델링 및 평가]**
    * [cite_start]**사용한 모델:** Logistic Regression, RandomForest, SVM, `AdaBoostClassifier`[cite: 1195, 1196].
    * [cite_start]**검증:** 불균형 데이터를 고려하여 `StratifiedK-Fold` 및 `RepeatedStratifiedKFold`를 사용하고, `GridSearchCV`로 하이퍼파라미터를 튜닝했습니다[cite: 1196].
    * [cite_start]**최종 모델:** Test 세트 정확도 0.73 [cite: 1237] [cite_start]및 F1-score 비교 시 가장 우수한 성능을 보인 **AdaBoostClassifier**를 채택했습니다 [cite: 1242] [cite_start](최적 매개변수: `learning_rate=0.1`, `n_estimators=50` [cite: 1227]).
* **[주요 분석 결과 (가설 검증)]**
    * [cite_start]**가설 기각:** 'CCTV', '안전표시판', '과속방지턱' 개수는 **오히려 사고가 날 지역에서 더 많았습니다**[cite: 1270, 1271, 1272].
    * [cite_start]**가설 채택:** '방호 울타리 길이'는 사고가 날 지역이 현저히 짧았고 [cite: 1273][cite_start], '옐로우 카펫 존'은 사고가 안 날 지역에 더 많이 설치되어 있었습니다[cite: 1274].
* **[결론 및 인사이트]**
    * [cite_start]CCTV, 과속방지턱 등은 사고 예방 목적이 아닌, **설치 의무를 위한 형식적 설치**이거나 사고 발생 후 *사후 대응*으로 설치되었을 가능성이 높다고 추론했습니다[cite: 1115, 1287, 1288].
    * [cite_start]**실질적 대안:** 사고 예방에 실질적 효과가 검증된 '방호 울타리'와 '옐로우 카펫'의 추가 설치를 제안했습니다[cite: 1294].
    * [cite_start]**위험 지역 도출:** 예측 결과, 성남시 73개 스쿨존 중 35개가 위험으로 예측되었으며, 특히 분당구(서현동, 정자동, 야탑동)에 위험 스쿨존이 밀집해 있음을 시각화 자료와 함께 제시했습니다[cite: 1245, 1282, 1295].

---

### 04. 머신러닝 프로젝트: 영화 개봉 전 정보 기반 IMDb 점수 예측

* [cite_start]**[프로젝트]** 영화 개봉 전 메타데이터를 활용한 IMDb 점수(흥행) 예측 머신러닝 모델 개발[cite: 882].
* **[개요]** 영화의 장르, 상영 시간, 감독, 배우 등의 정보로 IMDb 점수를 3개 등급(Hit/Average/Flop)으로 분류하는 예측 모델을 구축했습니다.
* [cite_start]**[데이터]** IMDb 비상업용 데이터셋(1,000만 개 이상 [cite: 888][cite_start])을 활용, 4개(basics, crew, principals, ratings [cite: 890, 891, 892, 893])의 데이터셋을 병합하고 전처리했습니다.
* **[피처 엔지니어링 및 전처리]**
    * [cite_start]결측값 처리(평균값 대체 [cite: 897][cite_start]), 정수형 변환 [cite: 898, 900] 등을 수행했습니다.
    * [cite_start]`genres_num`(장르 개수) [cite: 976][cite_start], `directors_count`(감독 수) [cite: 980][cite_start], `actor_count`(배우 수) [cite: 982][cite_start], `first_director`(첫 번째 감독 식별자) [cite: 978] 등 10개 이상의 파생 변수를 생성했습니다.
    * [cite_start]**타겟 변수:** `averageRating`(연속형)을 (1-3점: Flop, 3-6점: Average, 6-10점: Hit)의 3개 클래스('score')로 범주화했습니다[cite: 989, 991].
* **[모델링 및 평가]**
    * [cite_start]**사용한 모델:** Logistic Regression, RandomForest, AdaBoost, Bagging, GradientBoosting, `XGBClassifier`[cite: 995].
    * [cite_start]**튜닝:** `GridSearchCV`를 사용하여 각 모델의 최적 매개변수를 탐색했습니다[cite: 996].
    * [cite_start]**최종 모델:** 6개 모델 중 **XGBClassifier**가 Test 세트 정확도 **67%**로 가장 높은 성능을 기록했습니다[cite: 1018, 1019].
* **[결과 분석 및 한계]**
    * **낮은 정확도의 원인:**
        1.  [cite_start]**낮은 피처 상관관계:** 히트맵 분석 결과, 사용된 피처들 간의 상관관계가 매우 두드러지지 않았습니다[cite: 1022].
        2.  [cite_start]**클래스 간 불명확한 특성:** 'Hit Movie'(score 0)와 'Flop Movie'(score 2) 그룹 간 피처들의 평균/중앙값 차이가 통계적으로 유의미하지 않았습니다[cite: 1023].
    * **결론:** 현재 사용 가능한 피처(장르, 상영 시간, 스태프)만으로는 영화의 대중성(점수)을 예측하기에 한계가 있음을 확인했습니다.
    * [cite_start]**향후 개선:** 더 나은 예측을 위해 '영화 예산', '예고편 길이', '제작사', '등급' 등의 추가 피처가 필요함을 제언했습니다[cite: 1030, 1031].
```
