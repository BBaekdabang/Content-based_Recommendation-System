# Content-based_Recommendation-System

## 도서 추천시스템

---

### 가. Kinds of Similarity
<img width="190" img height="280" src="https://user-images.githubusercontent.com/113493692/217757684-7f36c286-3cbd-481b-bd19-89cdc5856c4a.png"><img width="190" img height="280" src="https://user-images.githubusercontent.com/113493692/217757951-c84cfb93-8d88-49c6-bec9-f754c5037db6.png"><img width="310" img height="280" src="https://user-images.githubusercontent.com/113493692/217758177-56c7c231-4650-42be-8644-209c4eba7720.png"><img width="230" img height="280" src="https://user-images.githubusercontent.com/113493692/217758309-3fc03e4e-1f36-4720-8f41-ca62d71e3ed7.png">


 - Cosine Similarity
  
   - Advantage
     1. 고차원 데이터일 경우 유리
     2. 크기가 유사도 점수에 영향을 미치지 않게 벡터를 정규화함
     3. 명확한 평점 데이터 불필요
    
   - Disadvantage
     1. 벡터간의 크기 차이를 고려하지 않음
     
 - Euclidean Distance
 
   - Advantage
     1. 계산의 간단함
     2. Binary 데이터가 아닌 경우에 사용 가능
     
   - Disadvantage
     1. 벡터간의 방향 차이를 고려하지 않음
     2. 데이터의 크기에 민감
     
 - Pearson Correlation
 
   - Advantage
   
     1. 두 데이터의 특징들 사의의 선형적 관계의 크기와 방향을 모두 고려
     2. Continuous, Binary 데이터에 모두 사용 가능
     
   - Disadvantage
   
     1. 비선형적인 관계가 있을 경우 사용 불가
     2. 데이터의 정규 분포를 가정
     
 - Jaccard Similarity
 
   - Advantage
   
     1. 계산의 간단함
     2. Binary 데이터일 경우 적합
     
   - Disadvantage
   
     1. 두 데이터의 크기의 차이를 고려하지 않음
     2. Continuous, Non-binary 데이터에 부적합
     
---

### 가. Dataset : YES24 인문, 자기계발, 소설, 에세이, 역사 카테고리 크롤링
<img width="1000" img height="280" src="https://user-images.githubusercontent.com/113493692/217748015-ba5f42b7-13ad-4a4d-b911-d365a9fbac68.png">

### 나. Methods

 - One-hot Encoding (Keyword Base)
 <img width="500" img height="400" src="https://user-images.githubusercontent.com/113493692/217763347-46af142f-a0a5-4371-8b57-899cd4b68a95.png">

 <img width="450" img height="380" src="https://user-images.githubusercontent.com/113493692/217762859-25c9ee39-1978-435e-8981-c8b951db3893.png"><img width="450" img height="380" src="https://user-images.githubusercontent.com/113493692/217762959-94fccdd1-f7ab-4776-8cad-67e81ef46831.png">

 - Tf-Idf (Overview Base)
 <img width="600" img height="480" src="https://user-images.githubusercontent.com/113493692/217764321-38a187bd-106e-4493-8417-a9ada6c45697.png">
 
 - Doc2Vec (Overview Base)
 <img width="800" img height="280" src="https://user-images.githubusercontent.com/113493692/218031285-9dba09f8-968f-4b18-ac4e-7b920a2ae44b.png">

 - SentenceBERT
 <img width="800" img height="200" src="https://user-images.githubusercontent.com/113493692/217783633-abc476fe-063a-4e2a-bd59-dfa899655e4e.png">
 <img width="800" img height="280" src="https://user-images.githubusercontent.com/113493692/218013994-21cdeb14-ba4a-44bd-b72b-955a40c5feca.png">
 
 ---
 
 ### 가. Reference
 - Doc2Vec : https://dailyheumsi.tistory.com/165
 - Similarity : https://github.com/SeongBeomLEE/Tobigs_Recommendation_System_Seminar/blob/main/Week2_Recommendation_Seminar_Code.ipynb
 - SentenceBERT : https://github.com/BM-K/KoSentenceBERT-ETRI
