# How to make Software Architecture
+ 여기서 말하고 있는 방법이 정답은 아니다.
+ Software Architecture를 작성하는 방법 중에 하나를 말한다.


## 1. Project Overview
1. Business Context Diagram   
   + Business Context Diagram을 작성해보면서 프로젝트와 관련된 Stakeholder들을 조사한다.
2. Stakeholder List
   + Business Context Diagram을 통해 Stakeholder 목록을 작성한다.
4. Business Goal
   + Stakeholder들의 Business Goal이 무엇인지 작성한다.
   + Business Goal은 System이 가져야 할 System Feature을 도출하는데 사용된다.

## 2. System Overview
1. System Context Diagram
   + Business Goal을 고려하여 System이 가져야 할 기능들에 대해 System Context Diagram을 작성한다.

<img src="https://user-images.githubusercontent.com/77768139/186164756-07239ca9-3ba6-4aa2-8cf9-144da6d991d4.jpg" width="800" height="800"/>

2. External Entity
   + System Context Diagram을 통해 External Entity 목록을 작성한다.
4. Interface List
   + System Context Diagram을 통해 Interface List 목록을 작성한다.
5. System Feature 
   + Interface List을 참고하여 System Feature들을 도출한다.

## 3. Architectural Driver
1. Use Case Model
   + Use Case Diagram
      + System Feature을 Use Case Digram으로 나타낸다.
      + Use Case Diagram을 작성해보면서 누락된 Actor, Feature가 있는지 확인한다.
   + Actor List
      + Use Case Diagram에서 작성한 Actor List를 작성한다. 
   + Use Case List
      + Use Case Diagram에서 작성한 Use Case List를 작성한다.
   + Use Case Description
      + 각 Use Case의 Description을 작성한다.
2.  
