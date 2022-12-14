# 얼굴형에 따른 모자 추천 프로그램

## 팀원 및 역할 
<img width="329" alt="역할" src="https://user-images.githubusercontent.com/102898911/206884020-55dc6a82-4dbe-4e3e-ac8c-522ccdee37cf.png">


## 개요 
사람들은 모두 다른 얼굴형을 가지고 있다. 긴 얼굴형을 가진 사람이 있는가 하면 각진 얼굴형을 가진 사람 등 사람들은 제각기 다른
얼굴형을 가지고 있다. 

![images](https://user-images.githubusercontent.com/102898911/201646447-3556aa79-4246-4d66-b576-428e8facbc04.jpg)

#### 출처:세계한인언론인협회 
<br> 그렇기 때문에 모자를 선택할 때도 모자의 패턴,재질 뿐만 아니라 모자의 종류 역시 고려해야할 사항 중 하나이다. 
얼굴형에 따라 잘 어울리는 모자가 있고, 그렇지 않은 모자가 있기 때문에 얼굴형에 맞는 모자를 선택하는 것은 매우 중요하다.

 그러나 매일 거울로 보는 본인의 모습을 객관적으로 판단하기 쉽지 않다. 나에게 꼭 맞는 모자를 고르기 위해서는 본인의 얼굴형이 어떤지 
알고 있어야 한다. 본 프로젝트에서는 이러한 어려움을 해결하고 사용자가 자신에게 맞는 모자를 선택하는 데 도움을 주고자 본 프로젝트를
과제로 선택하게 되었다. 

## 과제 목표 

### 1. 얼굴형을 4가지 유형으로 나누어 딥러닝 모델을 학습시킨다. 

얼굴형을 긴 얼굴형, 둥근 얼굴형, 역삼각형 얼굴형, 각진 얼굴형으로 나눈다. 
그리고 각 얼굴형을 가진 사람의 얼굴 사진으로 딥러닝 모델을 학습시킨다. 


### 2. 사용자가 입력한 사진을 사용해 딥러닝 모델이 얼굴형을 추측한다. 

사진 입력 화면을 만들어 사용자가 사진을 입력할 수 있도록 하고
사용자가 사진을 입력하면 딥러닝 모델이 이를 이용하여 얼굴형을 추측한다. 



### 3. 추측한 얼굴형을 기준으로 그에 맞는 모자를 추천한다. 

딥러닝이 추측한 얼굴형을 이용해 그에 맞는 모자를 추천하고 모자 이미지를 
사용자에게 보여준다. 


## 구현 

### 1. 딥러닝 학습 모델 선택

구글 Teachable Machine은 머신러닝 코드를 작성하지 않고 이미지를 머신러닝 모델에 학습시켜 사용할 수 있다는 장점이 있다. 
얼굴형 분류의 경우 미리 학습된 OpenCV 모델이 없기 때문에 Teachable Machine을 학습 모델로 선택하였다. 

#### Google Teachable Machine
<br> 

구글 Teachable Machine은 자바스크립트 머신러닝 라이브러리인 TensorFlow.js를 사용해 웹브라우저에서 만들어진 모델을 학습시키고 실행할 수 있다. 
Teachable Machine은 기존에 학습된 신경망을 이용해 자체 클래스를 만들면 이 클래스가 신경망의 마지막 레이어 또는 단계가 되는 전이 학습 기법을 
사용하고 있다. 

구글 Teachable Machine에서 모델을 만드는 과정은 다음과 같다. 


<img width="289" alt="단계1" src="https://user-images.githubusercontent.com/102898911/206883962-cb2d3b3a-c7a0-4696-bdf5-fbc7d29c71ea.png">

<img width="253" alt="단계2" src="https://user-images.githubusercontent.com/102898911/206883967-88d59d36-f045-4235-a5e3-0134557995a1.png">


<img width="266" alt="단계3" src="https://user-images.githubusercontent.com/102898911/206883970-eebfe5de-3947-4f4d-ad7b-fe5df17ab5b5.png">
출처 : Google Teachable Machine 





### 2. 자료 선택 

사람의 얼굴형은 다양하지만 그중 대표적으로 많은 사람들이 속하는 긴 얼굴, 둥근 얼굴, 역삼각형 얼굴, 각진 얼굴로 얼굴형을 나누었다.  
모델을 학습시키기 위한 자료가 많지 않으므로 각 자료들은 최대한 특징들이 부각되는 이미지로 준비하였다. 








### 3. 모델 학습 

선택된 자료를 사용하여 Techable Machine을 학습시킨다. 
<img width="698" alt="학습" src="https://user-images.githubusercontent.com/102898911/206856210-c0f68dc1-8053-4154-9d30-bb48209b65cb.png">


학습된 모델을 내보내기를 통해 tensorflow.js 로 다운로드 한다. 
<img width="617" alt="모델 내보내기 " src="https://user-images.githubusercontent.com/102898911/206856252-acf0e08c-01ed-4858-ac67-62300e9eefd3.png">

해당 모델을 Visual Studio Code를 사용하여 Html 파일을 만들어 임베디드 하여 사용한다. 



### 4. 모델의 웹 구현 

사용자가 사이트를 이용하기 전 사용법을 알리기 위해 사용법이 먼저 화면에 나오도록 하였다. 

<img width="339" alt="사이트 설명" src="https://user-images.githubusercontent.com/102898911/206855865-a7f29eee-ae7e-4f82-9a9a-736b55344be9.png">

기존의 Teachable Machine은 웹캠만을 사용하여 모델을 이용할 수 있다. 사용자가 이미지를 사용할 수 있도록 파일 입력 화면을 추가하였다. 

<img width="349" alt="파일 input" src="https://user-images.githubusercontent.com/102898911/206855963-2c60bb3f-9ccc-466a-97fd-f89d3b277fc7.png">

사용자의 얼굴형에 대한 텍스트를 추가하고 그에 맞는 모자 사진을 사용자에게 보여준다. 


<img width="373" alt="결과 화면 " src="https://user-images.githubusercontent.com/102898911/206855996-5aaea279-1370-465e-b0d6-d7799e2dc1c8.png">


## 개선 사항 

### 1.모델 정확도 개선 
딥러닝 모델은 많은 사진을 학습시킬 수록 모델의 성능이 향상된다. 
그러나 해당 모델은 데이터 수집의 어려움으로 충분한 양의 학습데이터를 확보하지 못하였다. 
그리하여 다음과 같이 제대로 된 예측을 하지 못하는 경우가 가끔 발생하였다. 

<img width="451" alt="개선사항" src="https://user-images.githubusercontent.com/102898911/206855041-a80b58c8-bc71-48b1-a9ad-f1728e72c9c9.png">





### 2. 사이트 디자인 개선 

사이트의 가시성을 위해 글꼴과 폰트 사이즈를 조정할 필요가 있으며 
사진의 크기를 통일하고 전체적인 텍스트와 사진의 비율을 조절할 필요가 있다. 
이러한 디자인 개선을 통해 사용자가 읽기 쉬운 사이트를 만들 수 있을 것이다. 

## 결론

구글의 Teachable Machine 머신을 이용하여 모자 추천 프로그램을 구현하였다. 
해당 프로그램을 통해 사용자는 자신의 얼굴형에 맞는 모자를 추천받을 수 있게 되었다.
몇 가지 개선사항이 있기는 하였지만 모델을 사용하는 데 큰 문제는 없었으며 
모델의 정확도와 웹 디자인 개선을 한다면 더 정확하고 사용하기 편할 것이다. 


## 출처 

https://teachablemachine.withgoogle.com/
