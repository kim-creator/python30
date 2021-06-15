앙상블(Ensemble) 모델

머신러닝 앙상블이란? 여러개의 머신러닝 모델을 이용해 최적의 답을 찾아내는 기법

여러 모델을 이용하여 데이터를 학습하고, 모든 모델의 예측결과를 평균하여 예측

앙상블 모델의 종류

보팅 (Voting) : 투표를 통해 결과를 도출

배깅 (Bagging) : 샘플 중복 생성을 통해 결과 도출

부스팅 (Boosting) : 이전 오차를 보완하면서 가중치를 부여

스태킹 (Stacking) : 여러 모델을 기반으로 예측된 결과를 통해 meta 모델이 다시 한번 예측

a=np.arange(36).reshape(3,4,3)

a

​

슬라이싱

arr=np.arange(1,37).reshape(3,4,3)

arr

​

arr[:,1:3,1:]

​

arr=np.arange(36).reshape(2,3,3,2)

arr

​

temp_arr = arr[np.newaxis, :, :, np.newaxis]

temp_arr.shape

​

temp_arr=arr[np.newaxis,...,np.newaxis]

temp_arr.shape

​

차원 쥐어짜기

개수가 1인 차원의 내용을 없애는 기법

temp_squeeze =np.squeeze(temp_arr)

temp_squeeze.shape

​

x=np.random.randint(15, size=(3,5))

x.shape

​

temp=np.ravel(x)

temp.shape
