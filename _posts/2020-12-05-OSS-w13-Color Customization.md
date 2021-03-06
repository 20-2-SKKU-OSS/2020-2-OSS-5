---	
layout: post	
title:  "[W13] Color Customization"	
author: ChoHyeonSu
categories: [ code ]	
tags: [what, project]
image: assets/images/ezgif-7-e43b2cae629a.gif
description: "Project Description"	
featured: true	
hidden: false	
rating: 4.5
---	

OSS_5 MEMBERS : Brian-Hwang, leedayun, Na-Hyeon-Oh, Jungseoyeon, ChoHyeonSu, jihye0

# 1단계: xml 파일
> CameraButton/camerabutton/src/main/res/values/colors.xml

먼저 xml 파일의 코드를 수정해서 원하는 색상을 불러와야 합니다.

- main_circle_color / main_circle_color_pressed / stroke_color / stroke_color_pressed 관련 부분

>Default

![스크린샷(411)](https://user-images.githubusercontent.com/65438056/101242769-ea19ee00-373e-11eb-8f53-11b99482759f.png)

이런 식으로 Default color가 정해져 있습니다. 

>Mycolor

<img width="259" alt="4" src="https://user-images.githubusercontent.com/65438056/101286218-97b6fb00-382c-11eb-94c7-08ed99ede74a.png">

이런 식으로 원하는 색상 #XXXXXX을 가져와서 저장합니다. 

- arc_color 관련 부분

>Default

![스크린샷(414)](https://user-images.githubusercontent.com/65438056/101242831-4977fe00-373f-11eb-89e5-1a845e3386d9.png)

이런 식으로 Default color가 정해져 있습니다.

>Mycolor

<img width="262" alt="5" src="https://user-images.githubusercontent.com/65438056/101286221-98e82800-382c-11eb-80c4-6bfa746a7c41.png">

이런 식으로 원하는 색상 #XXXXXX의 배열을 가져와서 저장합니다.

# 2단계: java 파일
> CameraButton/camerabutton/src/main/java/com/hluhovskyi/camerabutton/CameraButton.java
 
<img width="262" alt="5" src="https://user-images.githubusercontent.com/65438056/101286223-9a195500-382c-11eb-956b-41eef588adbc.png">

이런 식으로 원하는 색상을 가져와서 원하는 부분에 입힙니다.

#Example
- 순서대로 main_circle_color / main_circle_color_pressed / stroke_color / stroke_color_pressed / arc_color

> #000000 / #ffffff / #aa89bd / #7ecef4 / #000000 + #ffffff + #aa89bd + #7ecef4

> black / white / light_purple / skyblue / black + white + light_purple + skyblue

![ezgif com-gif-maker](https://user-images.githubusercontent.com/65438056/101243247-361a6200-3742-11eb-8eff-6ed970f6cc1d.gif)


> #daa8d7 / #ffa2cc / #f2e58c / #0000ff / #daa8d7 + #ffa2cc + #f2e58c + #0000ff

> light_pink / light_magenta / light_yellow / blue / light_pink + light_magenta + light_yellow + blue

![ezgif com-gif-maker (1)](https://user-images.githubusercontent.com/65438056/101243447-cd33e980-3743-11eb-99a4-2c4ee8cab500.gif)

> #cce198 / #cacaca / #606060 / #9bf6e0 / #cce198 + #cacaca + #606060 + #9bf6e0

> light_green / light_gray / drak_gray / mint / light_green + light_gray + drak_gray + mint

![ezgif com-gif-maker (2)](https://user-images.githubusercontent.com/65438056/101243537-78dd3980-3744-11eb-81b2-4eabd2f6b563.gif)



