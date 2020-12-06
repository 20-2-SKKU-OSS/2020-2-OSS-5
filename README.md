# ABOUT 2020-2-OSS-5 REPOSITORY 


## TEAM MEMBER
##### 저희 팀은 <br>

**&#9989; Hwang-Joon-Yong<br>
&#9989; Lee-Da-Yun<br>
&#9989; Im-Ji-Hye<br>
&#9989; Oh-Na-Hyeon<br>
&#9989; Jung-Seo-Yeon<br>
&#9989; Cho-Hyeon-Su<br>**

##### 까지 총 6명으로 구성되어 있습니다. <br>



# OSS-5's Project : Instagram Camera Button Commit

[&#9989; PROJECT Github Page](https://github.com/hluhovskyi/CameraButton?utm_source=android-arsenal.com&utm_medium=referral&utm_campaign=6877)

##### 저희는 `Instagram Camera Button'이라는 주제를 프로젝트로 선정하였습니다.
##### We selected 'Instagram Camera Button' as our project theme.

##### 이는 인스타그램 카메라 버튼에 다양한 visual한 기능을 추가할 수 있는 오픈 소스입니다.<br>
##### It is an open source that allows you to add various visual features to your Instagram camera buttons.

##### 저희는 이 버튼 기능에 사용자별 버튼 색 선정을 통한 Customization과 버튼 너비의 수정과 관련한 코드를 추가하여 이를 PR하는 방식으로 해당 프로젝트인 Instagram Camera Button Commit에 기여하는 것을 목표로 하고 있습니다.
##### We aim to contribute commit to Instagram Camera Button by adding user-specific Button-Color customization code and Button-Width customization code, and then Pulling Request to original project.

[&#9989; STATIC PAGE](https://20-2-skku-oss.github.io/2020-2-OSS-5/)<br>

##### 해당 프로젝트와 관련한 정보와 주차별 회의 정보는 [STATIC PAGE](https://20-2-skku-oss.github.io/2020-2-OSS-5/)를 참고하여 주시면 감사하겠습니다:smile:<br>

##### You can check our [STATIC PAGE](https://20-2-skku-oss.github.io/2020-2-OSS-5/) for more informations about the project and weekly contributions.



### Enhancement in project

#### CameraButton/camerabutton/src/main/java/com/hluhovvskyi/camerabutton/CameraButton.java

##### 개발 코드는 위와 같은 경로를 통해 확인하실 수 있습니다 !
##### You can check our Development Codes through above path.

- We add some explanation of main codes of this project
- Planning to customize in terms of color and width of button
- edit the width of button & range of colors
- ISSUE:: Since author of this project seems to deny pull request from the others, we enhance the code in our project temporarily.


### Wiki page
[&#9989; WIKI PAGE](https://github.com/20-2-SKKU-OSS/2020-2-OSS-5/wiki)<br>

##### 프로젝트의 진행 사항에 대한 details를 알고 싶으시다면 [WIKI PAGE](https://github.com/20-2-SKKU-OSS/2020-2-OSS-5/wiki)를 참고해주세요:)
##### We also posted our detailed progress on [WIKI PAGE](https://github.com/20-2-SKKU-OSS/2020-2-OSS-5/wiki)


## RESULTS OF OUR PROJECT

### Color Customization

##### Color.xml에 파스텔 계열, 원색 계열, 회색 음영 계열을 추가로 삽입하여 사용자가 원하는 색깔로 Custom할 수 있도록 했습니다.

##### We added some colors including pastel tone, primary tones and gray-base shades colors to "Color.xml" so that users can customize cameras based on their preferred color.


##### 색상의 이름을 my_color에서 "skyblue", "light_pink", "yellow", "blue", "light_gray" 등과 같이 컬러의 이름으로 지정하여 보다 직관적으로 색깔을 지정할 수 있도록 했습니다.

##### Additionally, we changed colors' name from my_color to general color names, such as "light_purple", "skyblue", and "light_gray", which allows users to assign colors in more intuitive way.


##### 다음을 이를 적용하여 light_purple, Skyblue, 그리고  light_gray 색상을 사용하여 Customizing 한 카메라입니다.

##### Following gif image is the result of customization using light_purple, skyblue and light_gray.

[&#9989; Color_Custom](https://user-images.githubusercontent.com/65438056/101243247-361a6200-3742-11eb-8eff-6ed970f6cc1d.gif)


### Stroke Width Customization

##### 스트로크 너비 부분은 setMainCircleRadius함수를 통해, 호의 너비 부분은 setStrokeWidth함수를 통해 결정된다는 것을 확인했습니다.

##### We confirmed that the width of the stroke is determined by the setMainCircleRadius function and the width of the arc by the setStrokeWidth function.

##### 함수 내부에서 사용하는 변수들의 값은 dimens.xml 안에 저장되어 있었고, default 값으로 저장되어 있는 값들을 변경하였습니다. 

##### The values of the variables used inside the function were stored within dimens.xml, and the values stored as default values were changed.

##### 버튼 반지름의 크기를 24dp에서 30dp로 키워서 사용자가 한 눈에 알아볼 수 있고 쉽게 누를 수 있도록 하게 했습니다.

##### The size of the button radius has been increased from 24 dp to 30 dp, making it recognizable and easy for users to press.

##### 호의 크기는 12dp에서 15dp로 키워서 버튼 위에 색이 나타날때 사용자 본인이 선택한 색을 잘 볼 수 있도록 하게 했습니다.

##### The arc size was raised from 12dp to 15dp so that you could see the color you chose when the color appeared on the button.


[&#9989; Width_Custom1](https://user-images.githubusercontent.com/65438056/101273506-5d703e00-37d9-11eb-86ca-9d6a7e6b2c97.png)  [&#9989; Width_Custom2](https://user-images.githubusercontent.com/65438056/101273507-5ea16b00-37d9-11eb-8fdc-8f15001f1a0f.png)  [&#9989; Arc_Custom](https://user-images.githubusercontent.com/65438056/101273508-5f3a0180-37d9-11eb-9822-96b125c48bc1.png)



