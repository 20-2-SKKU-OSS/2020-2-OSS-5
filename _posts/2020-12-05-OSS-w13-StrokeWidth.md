---   
layout: post   
title:  "[W13] Button Width"   
author: jihye0
categories: [ code ]   
tags: [what, project]
image: https://user-images.githubusercontent.com/73014113/101245739-40dcf300-3752-11eb-9412-fd500bb743a9.png
description: "Project Description"   
featured: true   
hidden: false
rating: 4.5
---   

OSS_5 MEMBERS : Brian-Hwang, leedayun, Na-Hyeon-Oh, Jungseoyeon, ChoHyeonSu, jihye0

# 1단계: xml 파일
> CameraButton/camerabutton/src/main/res/values/dimens.xml

코드 분석을 통해 stroke 너비 부분은 setMainCircleRadius함수를 통해 결정됨을 알 수 있었습니다. 
setMainCircleRadius 함수 내부에 있는 변수인 mMainCircleRadius를 이용해 버튼의 너비를 조절하고자 했습니다. 
또한 setStrokeWidth 함수는 버튼에 나타나는 색의 넓이를 조절하는 함수임을 알 수 있었습니다. 
따라서 setStrokeWidth 함수 내부의 변수인 mStrokeWidth를 분석했습니다. 

Default value - 28dp/@dimen/cb_main_circle_radius_default

![스크린샷(411)](https://user-images.githubusercontent.com/73014113/101245739-40dcf300-3752-11eb-9412-fd500bb743a9.png)

Default value - 12dp/@dimen/cb_stroke_width_default

![스크린샷(410)](https://user-images.githubusercontent.com/73014113/101245801-bcd73b00-3752-11eb-971c-8278e65bda55.png)

[버튼을 누르기 전]
이런 코드 분석을 거쳐 default값을 변경한다면 버튼의 지름과 너비가 변할 것이라고 생각했습니다. 
먼저 버튼 반지름의 크기를 24dp에서 30dp로 증가시켜 버튼의 크기를 키웠습니다. 
버튼의 크기를 다음과 같이 키운 이유는 사용자가 한 눈에 알아볼 수 있고 쉽게 누를 수 있도록 하기 위함이었습니다. 

또한 width의 변수값을 12dp에서 15dp로 수정하였습니다. 
이렇게 width 값을 증가시킨 이유는 버튼 위에 색이 나타날때 사용자 본인이 선택한 색을 잘 볼 수 있도록 하기 위해서였습니다.

Default value - 24dp/@dimen/cb_main_circle_radius_expanded_default

![스크린샷(414)](https://user-images.githubusercontent.com/73014113/101245856-163f6a00-3753-11eb-8b52-4d0d76cb4609.png)

[버튼을 누른 후]

먼저 버튼 반지름의 크기를 24dp에서 20dp로 감소시켜 버튼의 크기를 키웠습니다. 
버튼의 크기를 다음과 같이 감소시킨 이유는 사용자가 버튼을 눌렀을때 그 변화를 조금 더 극적으로 한 눈에 알아볼 수 있도록 하기 위함이었습니다. 

또한 width의 변수값을 4dp에서 5dp로 수정하였습니다. 
이렇게 width 값을 수정한 이유는 버튼을 누른 후 버튼 위에 색이 나타날때 사용자 본인이 선택한 색을 잘 볼 수 있도록 하기 위해서였습니다.

>Changed 

cd_layout_width_defalut와 cd_layout_height_default값이 120dp라고 정의되어있습니다. 

![스크린샷(413)](https://user-images.githubusercontent.com/73014113/101245922-6e766c00-3753-11eb-8abc-6c0974379545.png)


