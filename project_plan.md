# 얼굴형에 따른 모자 추천 프로그램


## 1.팀원 및 업무분담

![팀원 및 역할분담](https://user-images.githubusercontent.com/102898911/201619368-d7dc6b88-3b67-4e74-98c5-6f049f3e9766.png)


##  2.과제 요약
 
본 프로젝트에서는 teachable머신의 딥러닝모델을 이용하여 4가지의 다른 얼굴형을 학습하고 학습된 모델을 tensorflow.js 모델로 변환하여 
웹사이트에 접속한 사용자가 얼굴 사진을 입력하면 딥러닝모델이 여기서 얼굴형을 분류하고 분류된 얼굴형에 적합한 모자를 추천해주는 시스템이다. 


##  3. 과제 개요 및 과제 선택 동기 
사람들은 모두 다른 얼굴형을 가지고 있다. 긴 얼굴형을 가진 사람이 있는가 하면 각진 얼굴형을 가진 사람 등 사람들은 제각기 다른
얼굴형을 가지고 있다. 

![images](https://user-images.githubusercontent.com/102898911/201646447-3556aa79-4246-4d66-b576-428e8facbc04.jpg)

#### 이미지[1] 출처:세계한인언론인협회 
<br> 그렇기 때문에 모자를 선택할 때도 모자의 패턴,재질 뿐만 아니라 모자의 종류 역시 고려해야할 사항 중 하나이다. 
얼굴형에 따라 잘 어울리는 모자가 있고, 그렇지 않은 모자가 있기 때문에 얼굴형에 맞는 모자를 선택하는 것은 매우 중요하다.

 

그러나 매일 거울로 보는 본인의 모습을 객관적으로 판단하기 쉽지 않다. 나에게 꼭 맞는 모자를 고르기 위해서는 본인의 얼굴형이 어떤지 
알고 있어야 한다. 본 프로젝트에서는 이러한 어려움을 해결하고 사용자가 자신에게 맞는 모자를 선택하는 데 도움을 주고자 본 프로젝트를
과제로 선택하게 되었다. 


## 4. 과제 목표

본 프로젝트에서는 다음을 과제의 목표로 설정하였다. 
1) 딥러닝모델이 사용자가 입력한 얼굴 사진의 얼굴형을 분류할 수 있도록 학습시킨다. 
2) 얼굴형의 분류는 역삼각형 얼굴형, 둥근 얼굴형, 각진 얼굴형, 긴 얼굴형으로 나눈다. 
3) 사용자가 사진을 입력하면 딥러닝모델이 얼굴형을 분석하고 사용자의 얼굴형에 맞는 모자를 추천한다. 

## 5. 결과물 
### 1) 예상 결과물

사용자가 얼굴 사진을 입력하면 딥러닝모델이 이를 분석하여 얼굴형을 분류한다. 얼굴형에 따라 어울리는 모자를 
미리 데이터로 등록하여 얼굴형 분류가 끝나면 미리 등록한 모자 데이터와 사용자가 입력한 얼굴 사진의 얼굴형을 매치하여 어울리는 모자를
사용자에게 텍스트와 사진으로 보여준다.

### 2) 기대효과 및 활용방안

모자를 구매할 때 직접 써보지 않고 인터넷으로 주문하는 사람들이 많다. 이때의 문제점은 나에게 어울리는지 어울리지 않는지 알 수가 없다는 것이다. 
모자를 살때는 색상이나 재질 뿐만 아니라 모자의 종류 자체도 매우 중요하다. 그리고 모자의 종류별로 나에게 어울리는지 혹은 어울리지 않는지는 
얼굴형에 따라 다르다. 그러나 본인의 얼굴을 객관적으로 판단하기는 매우 어렵다. 따라서 딥러닝모델이 이러한 판단을 대신해주고 거기서 더 나아가 
얼굴형에 맞는 모자까지 추천해준다면 사용자가 모자를 구매하는 데 있어서 고민을 덜 수 있을 것이라고 생각된다. 또한 모자를 판매하는 업체에서는 
본 프로젝트의 프로그램과 판매중인 모자를 연결하여 소비자가 얼굴형을 파악한 뒤 바로 그에 맞는 상품을 구매할 수 있도록 판매중인 상품을 추천하는 
방식으로 고객의 불편함을 덜 수 있을 것이다. 


## 6. 수행일정 및 작업 도구 

### 1) 수행일정

![제목을 입력해주세요_-001](https://user-images.githubusercontent.com/102898911/201655965-3e626c04-e49a-40bf-bd75-a8327b8b1847.jpg)



### 2) 작업 도구 

<img width="587" alt="구분" src="https://user-images.githubusercontent.com/102898911/202902749-9c14c321-125d-4572-8a8c-054aaddfdbaa.png">



## 7. 참고문헌 

이미지[1] 세계한인언론인협회,  [https://www.google.com/imgres?imgurl=https%3A%2F%2Fvelog.velcdn.com%2Fimages%252Fsjongyuuu%252Fpost%252Fb1b4aff9-18c2-46b8-9235-386a780b8d05%252Fai%25ED%258E%25B8-%25EC%25BA%25A1%25EC%25B2%2598.JPG&imgrefurl=https%3A%2F%2Fvelog.io%2F%4[0sjongyuuu%2FDeep-Learning-%25EC%2596%25BC%25EA%25B5%25B4%25ED%2598%2595-%25EB%25B6%2584%25EB%25A5%2598-%25EB%25AA%25A8%25EB%258D%25B8-%25EB%25AA%25A8%25EB%2](http://www.okja.org/saseol/129634)58D%25B8-%25EC%25A0%2595%25EC%259D%2598-%25EB%25B0%258F-Data-Set-%25EA%25B5%25AC%25EC%25B6%2595&tbnid=wOGglkgpDE4lEM&vet=12ahUKEwiXj-K0xK37AhXjRvUHHeUvBvMQMyg-egQIARBa..i&docid=e9YCFFXKle245M&w=870&h=419&q=%EC%96%BC%EA%B5%B4%ED%98%95%20%EB%AA%A8%EC%9E%90&hl=ko&ved=2ahUKEwiXj-K0xK37AhXjRvUHHeUvBvMQMyg-egQIARBa](http://www.okja.org/saseol/129634)
