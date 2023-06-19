# WaferDefectClasscification(By 2D-CNN, Keras)
## 산업공학종합설계 프로젝트

![image](https://user-images.githubusercontent.com/88662101/230546089-14fb8793-fd27-4062-946f-8daa17417dc7.png)  

- 프로젝트 선정 이유 : 2022 차량용 반도체 수급 문제와 이에 따른 반도체 수율 이슈 해결을 위한 불량 이슈 해결

<br>
<br>
<br>

![image](https://user-images.githubusercontent.com/88662101/230546209-e4bd8ec1-372e-4b14-8022-aedd208b0054.png)  


- 데이터 전처리 - 데이터 구성 파악(시각화)  
- 웨이퍼 맵 : 2Dim array 형태로 0,1,2로 구성 
- Die-Size, Lot-name – Wafer 25EA 당, 1 Lot  
- waferindex – Wafer 별 ID
- trainTestLabel – Train/Test 구분  
- failureType – Defect 유형(Traget Data)  

<br>
<br>
<br>

![image](https://user-images.githubusercontent.com/88662101/230546607-54f0e346-3c60-4ee0-9c86-849d0f2ac407.png)  
- 불량 유형의 시각화  

<br>
<br>
<br>
<br>

![image](https://user-images.githubusercontent.com/88662101/230546662-2b095698-bd47-47bc-afe3-f5549ce4744d.png)  
- Auto-Encoder : Image Data를 더욱 선명하게 하기 위해서 만든 전처리 -> 데이터 품질 향상

<br>
<br>
<br>
<br>

![image](https://user-images.githubusercontent.com/88662101/230546810-d1ca473c-0b95-45ae-9d58-e6d6e8bfc8d7.png)  
- Edge case의 Net-Die가 가장 높았고, 데이터 불균형으로 인해 데이터 증강으로 이를 해소(Data 증감 기법)

<br>
<br>
<br>

![image](https://user-images.githubusercontent.com/88662101/230546952-5b856980-e163-48dd-9d24-4e2ff84f3fa0.png)  
- 2D CNN(Keras)을 활용한 분류 모델 개발  

<br>
<br>
<br>
<br>

![image](https://user-images.githubusercontent.com/88662101/230547003-5f732b84-daf1-4c3b-b7d5-967729ca8a61.png)  
- BAD Class는 edge case 2가지를 의미  
- 증강 갯수에 따른 예측 정확도 93% 달성


<br>
<br>

# Bcak-End Dev   

### Skill  
- Flask로 API를 생성 및 Ngrok 배포  
- 개당 웨이퍼의 불량을 선별할 수 있는 AI 모델을 통해 검출  


