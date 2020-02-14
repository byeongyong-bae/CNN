# CNN        
   
![CNN1](https://user-images.githubusercontent.com/59756209/74507272-435e2a00-4f3f-11ea-8b08-ce13d24bf91c.PNG)   
    
Convolution Neural Network(CNN)은 image 분야를 다루기에 optimization된 AI Neural Network이다.   
CNN은 크게 Convolution Layer와 Pooling Layer으로 구성되어 있다.    
   
## 1. Convolution   
   
![convolution](https://user-images.githubusercontent.com/59756209/74508508-8cfc4400-4f42-11ea-9bc7-a6ec8622344f.PNG)   
   
Convolution Layer는 Convolution 연산을 통해서 이미지의 특징을 추출한다.   
합성곱, Kernel, filter, Window Size라고도 불립니다.   
X x X 행렬을 Y x Y크기의 이미지 행렬과 곱해서 모두 거하는 수학 연산자이다.   
행렬곱의 결과로 이미지의 행렬의 부분 값들은 모두 더해져 하나의 값으로 모아진다.   
Convoultion에서 kernel의 종류에 따라 원본 image의 feature들이 다양하게 추출된다.   
   
## 2. Pooling   
   
![pooling](https://user-images.githubusercontent.com/59756209/74508927-a05bdf00-4f43-11ea-8f1b-209669d753b8.PNG)   
   
Pooling Layer는 차원을 축소하는 연산을 수행한다.   
Pooling 종류에는 Max Pooling, Average Pooling, Min Pooling이 있다.   
Max Pooling은 이미지의 X x X 크기 부분에서 가장 큰 값을 추출해서 원본 이미지의 X x X 개의 값을 1개의 값으로 축소합니다.   
Average Pooling, Min Pooling은 각각 평균, 최소값으로 축사한다.   
이미지의 차원을 축소함으로써 연산량을 감소시킬 수 있고, 이미지의 가장 강한 feature만을 extraction하는 feature extraction effect가 있다.   
   
## 3. Fully Connected   
분류 문제이면, Pooling으로 축소된 값들을 Neural Network 구조인 Fully Connected Layer의 input으로 들어가서 Softmax 분류를 수행하게 된다.   
