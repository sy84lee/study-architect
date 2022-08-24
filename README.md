# How to make Software Architecture
+ 여기서 말하고 있는 방법이 정답은 아니다.
+ Software Architecture를 작성하는 방법 중에 하나를 말한다.


## 1. Project Overview
1. Business Context Diagram
   + Business Context Diagram을 작성해보면서 프로젝트와 관련된 Stakeholder들을 조사한다.
2. Stakeholder List
   + Business Context Diagram을 통해 Stakeholder 목록을 작성한다.
3. Business Goal
   + Stakeholder들의 Business Goal이 무엇인지 작성한다.
   + Business Goal은 System이 가져야 할 System Feature을 도출하는데 사용된다.

## 2. System Overview
1. System Context Diagram
   + Business Goal을 고려하여 System이 가져야 할 기능들에 대해 System Context Diagram을 작성한다.

<img src="https://user-images.githubusercontent.com/77768139/186164756-07239ca9-3ba6-4aa2-8cf9-144da6d991d4.jpg" width="800" height="800"/>

2. External Entity
   + System Context Diagram을 통해 External Entity 목록을 작성한다.
2. Interface List
   + System Context Diagram을 통해 Interface List 목록을 작성한다.
2. System Feature 
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
2. Quality Attribute Scenario
   + Quality Attribute는 매우 중요하다.
   + System 또는 Software의 Architecture을 정하는 Quality Attribute이다.
   + Quality Attribute Scenario의 수가 늘어날수록 System 또는 Software의 Architecture를 작성하는 것은 어렵겠지만, 그만큼 단단한 System 또는 Software를 만들 수 있을 것이라 생각한다.
   + QA Scenario List
   + QA Scenario
   
## 4. Top Level Design Description
   + Top Level Design은 각각의 Component들로 구성되어 있으며, 각 Component들은 하위 Component들로 구성되어 질 수 있다.
   + Top Level Design은 Reference Architecture을 참고하거나 Architecture Pattern을 적용하는 것이 쉽게 시작할 수 있는 방법이다.
   + 여기서는 Layred Pattern을 적용하여 진행하였다.
1. Structure View
   + Static Structure Diagram을 작성하고, Static Structure Diagram을 구성하고 있는 각 Component의 Description을 작성한다.
   + Static Structure Diagram
   + Component Description
2. Behavior View
   + Top Level 수준에서 Behavior Diagramd을 작성한다.
3. Deployment View
   + Deployment Diagram을 작성한다.
4. Design Decision
   + Architecture을 작성할 때 필요한 Design Decision을 작성한다.
   
## 5. Component Level Design Description
   ++ 각 컴포넌트의 설계를 작성한다.
   ++ Class들로 구성되어 있으며 Design Pattern이 적용될 수 있다.
1. Static Structure Diagram
   ++ Class Diagram을 통해 Static Structure View를 보여준다.
   ++ 적용된 Design Pattern이 표현될 수 있다.
2. Behavior Diagram
   + Sequence Diagram을 통해 Behavior을 보여준다.

## 6. Architecture Evaluation
   ++ 각 Use Case들이 구현되어 있는지, 어느 요소에 포함이 되어 있는지 추적확인을 한다.
