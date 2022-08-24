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
   <img src="https://user-images.githubusercontent.com/77768139/186418814-1ba3cf5e-411f-4480-a33d-06d430761d65.JPG" width="500" height="300"/>
   
3. Interface List
   + System Context Diagram을 통해 Interface List 목록을 작성한다.
   <img src="https://user-images.githubusercontent.com/77768139/186418950-91616c49-1f0a-4fcc-82be-8602785f0fa2.JPG" width="500" height="300"/>

4. System Feature 
   + Interface List을 참고하여 System Feature들을 도출한다.
   <img src="https://user-images.githubusercontent.com/77768139/186419216-5a2d73d8-1f61-4b8b-8057-3a0b6a603ee9.JPG" width="500" height="250"/>


## 3. Architectural Driver
1. Use Case Model
   + Use Case Diagram
      + System Feature을 Use Case Digram으로 나타낸다.
      + Use Case Diagram을 작성해보면서 누락된 Actor, Feature가 있는지 확인한다.
   
   + Actor List
      + Use Case Diagram에서 작성한 Actor List를 작성한다.
      <img src="https://user-images.githubusercontent.com/77768139/186419025-0d75bb45-ce4b-4a0b-8b55-629137867a09.JPG" width="500" height="250"/>
   
   + Use Case List
      + Use Case Diagram에서 작성한 Use Case List를 작성한다.
      <img src="https://user-images.githubusercontent.com/77768139/186419338-686121b2-15d5-4322-8bb1-0d01bc8ebba1.JPG" width="500" height="250"/>
   
   + Use Case Description
      + 각 Use Case의 Description을 작성한다.
      <img src="https://user-images.githubusercontent.com/77768139/186419409-a3f845d3-701b-4d61-8fb7-a2aaca8fad54.JPG" width="500" height="550"/>

2. Quality Attribute Scenario
   + Quality Attribute는 매우 중요하다.
   + System 또는 Software의 Architecture을 정하는 Quality Attribute이다.
   + Quality Attribute Scenario의 수가 늘어날수록 System 또는 Software의 Architecture를 작성하는 것은 어렵겠지만, 그만큼 단단한 System 또는 Software를 만들 수 있을 것이라 생각한다.
   
   + QA Scenario List
   <img src="https://user-images.githubusercontent.com/77768139/186421711-a4fd9564-48d4-4672-9f23-e8dce73c731f.JPG" width="500" height="300"/>
   
   + QA Scenario
   <img src="https://user-images.githubusercontent.com/77768139/186421792-26bec5c8-7556-48ca-bb77-bb74dd13cd1d.JPG" width="500" height="300"/>
   
   
## 4. Top Level Design Description
   + Top Level Design은 각각의 Component들로 구성되어 있으며, 각 Component들은 하위 Component들로 구성되어 질 수 있다.
   + Top Level Design은 Reference Architecture을 참고하거나 Architecture Pattern을 적용하는 것이 쉽게 시작할 수 있는 방법이다.
   + 여기서는 Layred Pattern을 적용하여 진행하였다.
   
1. Structure View
   + Static Structure Diagram을 작성하고, Static Structure Diagram을 구성하고 있는 각 Component의 Description을 작성한다.
   + Static Structure Diagram
   <img src="https://user-images.githubusercontent.com/77768139/186421950-47afb3a5-d92d-4a78-8741-6e9fdefeb105.jpg" width="700" height="700"/>
         
2. Behavior View
   + Top Level 수준에서 Behavior Diagramd을 작성한다.
   <img src="https://user-images.githubusercontent.com/77768139/186422084-0730ba2a-abe9-4eb6-986d-abf09e4df703.jpg" width="500" height="700"/>
   
3. Deployment View
   + Deployment Diagram을 작성한다.
   <img src="https://user-images.githubusercontent.com/77768139/186422137-24fbd46b-4129-494a-a12a-c726aa3897a7.jpg" width="700" height="600"/>
   
4. Design Decision
   + Architecture을 작성할 때 필요한 Design Decision을 작성한다.
   + Design Decision List
   <img src="https://user-images.githubusercontent.com/77768139/186426243-a57ae99a-4e83-4f09-a2c9-0e45a6b6ac46.JPG" width="500" height="200"/>
   
   + Design Decision
   <img src="https://user-images.githubusercontent.com/77768139/186426367-33edb5d9-c070-4bb9-a5ac-48d131f66bd6.JPG" width="500" height="300"/>
   
## 5. Component Level Design Description
   + 각 컴포넌트의 설계를 작성한다.
   + Class들로 구성되어 있으며 Design Pattern이 적용될 수 있다.
   
1. Static Structure Diagram
   + Class Diagram을 통해 Static Structure View를 보여준다.
   + 적용된 Design Pattern이 표현될 수 있다.
   <img src="https://user-images.githubusercontent.com/77768139/186426611-1ec122f1-66aa-42b0-993c-97fcdc2e66e8.jpg" width="800" height="700"/>
   
2. Behavior Diagram
   + Sequence Diagram을 통해 Behavior을 보여준다.
   <img src="https://user-images.githubusercontent.com/77768139/186426777-c886f692-035c-476a-8a69-6a1f04f46563.jpg" width="800" height="700"/>

## 6. Architecture Evaluation
   + 각 Use Case들이 구현되어 있는지, 어느 요소에 포함이 되어 있는지 추적확인을 한다.
   <img src="https://user-images.githubusercontent.com/77768139/186426469-7af11a30-4758-4988-8e84-f18ce47993b9.JPG" width="600" height="500"/>
