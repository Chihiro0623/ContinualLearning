# Study


## [CL연구base정리.pptx](https://github.com/Chihiro0623/ContinualLearning/blob/main/Study/CL%EC%97%B0%EA%B5%ACbase%EC%A0%95%EB%A6%AC.pptx)
powered by [@joosunki](https://www.github.com/joosunki)


## 논문
https://github.com/xialeiliu/Awesome-Incremental-Learning

### [iCaRL Incremental Classifier and Representation Learning](https://github.com/Chihiro0623/ContinualLearning/blob/main/Study/Papers/iCaRL%20Incremental%20Classifier%20and%20Representation%20Learning.pdf)  
Continual Learning 중 Class-Incremental 방식의 가장 기초적인 원리를 제안한 논문이다. 이 논문에서 제안하는 Class-Incremental의 세 가지 특성에는 1. 다른 class의 유입을 학습할 수 있어야 한다. 2. 지금까지 학습된 class에 대해서 일정 수준 이상의 classification을 수행할 수 있어야 한다. 3. 계산 요구사항과 메모리를 일정 수준 이내에서만 요구해야 한다. 따라서 이 논문에서 제안하는 iCarl은 1. nearest-mean-of-examplars rule을 통해 classification을 수행하고, 2. herding에 따른 prioritized exemplar selection을 수행하고, 3. knowledge distillation과 prototype rehearsal의 두 가지 방식을 전부 활용하여 학습한다. 이렇게 iCarl로 학습하게 되면 각 class가 언제 입력되었는지와 관계없이 모든 class에 대해 비슷한 분포로 예측을 하게 되고, 다른 class-incremental 모델들보다 더 좋은 결과를 내게 된다.
