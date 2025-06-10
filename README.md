# 영상 데이터 분류
## 깨진 달걀 분류하기
-영상 데이터 분류(깨진계란, 빈 계란, 멀쩡한 계란 영상 분류)\n
-영상데이터 분류(깨진 계란, 빈 계란, 멀쩡한 계란 영상 분류)\n
-입력 변수  :  예40*40 픽셀영상\n
-출력 변수 :  ‘crack’, ‘empty’, ‘good’ (깨진 계란, 빈 계란, 멀쩡한 계란 )
## 데이터 설명
-데이터 개수 : 총 569장의 이미지파일 (훈련데이터 542개, 테스트데이터 27개)\n
-속성 : 3개( ‘crack’, ‘empty’, ‘good’)\n
-training data, test data 비율 : training data 80%, test data 20%\n
-검증 데이터 비율 : 학습데이터 중 20%
## 전처리과정
-OpenCV(이미지 크기 조정), Numpy 전처리
## 테스트 결과
![image](https://github.com/user-attachments/assets/2d0def02-3bff-4994-8bac-f1bc31ef1dea)
![image](https://github.com/user-attachments/assets/cef38b33-3f35-4313-b6b4-e1f1a57edaa2)
![image](https://github.com/user-attachments/assets/a027bd65-c91a-4959-a563-8b680a716dfc)

## 최종 하이퍼 파라미터
- Layer수: 11\n
- 활성화함수: relu, softmax\n
- 손실함수: sparse_categorical_crossentropy\n
- 뉴런 수: 64-128-256\n
- Kernal크기: 3x3, 2x2, 3x3\n
- Epoch : 100\n
- Batch_size : 100\n
- 옵티마이저: adam\n
일때가 영상 27개중 24개를 분류함으로써 3차 테스트의 구조가 가장 좋다.




