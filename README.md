# Objection-Detection  
● 객체 인식이란?  
● 영상에서 찾고자 목적하는 물체의 위치를 찾아내고 분류하는 과정을 말한다.  
●  얼굴 인식, 스마트 팩토리, 구조물 관리 등 다양한 분야에서 응용되고 있다.

<img src="https://user-images.githubusercontent.com/98728682/153541046-76ce92af-64ae-40da-b49f-b80de477a92c.jpg" width="480" height="230">

## Objection-Detection의 구조  
● 객체인식의 구조는 크게 One Stage와 Two Stage로 나뉜다.  

● One Stage는 객체의 위치와 종류를 한번에 찾아내는 구조이다. 대표적인 모델로 YOLO(You Only Look Once)가 있다.    
● 빠르지만 정확도가 약간 떨어진다.  

● Two Stage는 객체의 위치를 먼저 찾고 이후에 찾은 객체가 무엇인지 찾아내는 구조이다. 대표적인 모델로 Faster R-CNN이 있다.  
● 느리지만 정확도가 좋다.

## Faster R-CNN
● 전체 이미지를 CNN에 통과시켜 feature map을 생성한다.  

● RPN(Region Proposal Network)을 이용해서 객체가 있을법한 영역 800개를 찾아낸다.  

● RPN의 결과로 원래 이미지 위에 어디쯤에 객체가 있을지에 대한 정보가 나오므로 이것을 이용해 ROI(Region of Interest) Pooling을 진행함.  

● 총 4개의 결과가 나옴 RPN의 Classification & Localization과 최종 끝 부분의 Classification &  Localization이 나온다.
<img src="https://user-images.githubusercontent.com/98728682/153544846-fe9ca3dc-54cf-4186-8931-4872c5635804.png" width="480" height="320">  
]
