# Objection-Detection  
● 객체 인식이란?  
● 영상에서 찾고자 목적하는 물체의 위치를 찾아내고 분류하는 과정을 말한다.  
●  얼굴 인식, 스마트 팩토리, 구조물 관리 등 다양한 분야에서 응용되고 있다.

<img src="https://user-images.githubusercontent.com/98728682/153541046-76ce92af-64ae-40da-b49f-b80de477a92c.jpg" width="480" height="230">

## Objection-Detection의 구조  
● 크게 One Stage와 Two Stage로 나뉜다.  
● One Stage는 객체의 위치와 종류를 한번에 찾아내는 구조이다. 대표적인 모델로 YOLO(You Only Look Once)가 있다. 빠르지만 정확도가 약간 떨어짐.  
● Two Stage는 객체의 위치를 먼저 찾고 이후에 찾은 객체가 무엇인지 찾아내는 구조이다. 대표적인 모델로 Faster R-CNN이 있다. 느리지만 정확도가 좋음.
