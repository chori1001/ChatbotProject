# ChatbotProject
챗봇 프로젝트

빅데이터 기반 사용자 맞춤형 여행지 추천 챗봇 


KoGP2-Chatbot 사용 간 유의사항
gluonnlp 설치 간에 오류 발생 -> 비쥬얼 스튜디오 설치로 해결
(비쥬얼 스튜디오 -> C++  빌더만 설치하면 OK)

cuda 사용 간에 num_worker = 0 (colab 진행 후 세이브 데이터로 모델 실행만 진행.)

KoChat 실행 간 유의사항
폴더 경로 유의. 실행이 아예 되지 않는 경우 발생


KoChat 학습 진행 간 main loop 오류는 matplot으로 인한 것.
matplot.use('Agg')를 해주면 오류가 나지 않고 학습이 진행 됨.



argmax(): argument 'input' (position 1) must be Tensor, not str 오류
-> 트랜스포머 버전 문제. kogpt2가 설치했던 2번대 버전으로 설치를 해야 함 (파이토치, 쿠다와는 연관이 없음.)


kochat 에서 DistanceClassifier(intent 분류) 간에 lstm이 아닌 cnn을 사용한 이유는 LSTM보다 CNN의 Feature들이 클래스별로 훨씬 잘 구분되는 것을 개발자가 트레이닝 후 확인한 결과.
