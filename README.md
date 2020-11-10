# ChatbotProject
챗봇 프로젝트

빅데이터 기반 사용자 맞춤형 여행지 추천 챗봇 


KoGP2-Chatbot 사용 간 유의사항
gluonnlp 설치 간에 오류 발생 -> 비쥬얼 스튜디오 설치로 해결
cuda 사용 간에 num_worker = 0 (colab 진행 후 세이브 데이터로 모델 실행만 진행.)

KoChat 실행 간 유의사항
폴더 경로 유의. 실행이 아예 되지 않는 경우 발생


KoChat 학습 진행 간 main loop 오류는 matplot으로 인한 것.
matplot.use('Agg')를 해주면 오류가 나지 않고 학습이 진행 됨.
