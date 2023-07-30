# Experiment 1-2  
## 가정
학습 과정에서 N개의 Class 중 X개의 Class만을 노출시키면 Top-1 Accuracy가 X/N(%)가 될 것이다  

[이전의 실험](https://github.com/Chihiro0623/ContinualLearning/tree/main/Experiments/experiment1)에서는 총 50000개의 데이터 중 N개의 Class에 해당하는 데이터, 즉 N*500개의 데이터만을 이용했으나, 이번 실험에는 데이터를 중복시키는 방법으로 N의 수와 관계없이 50000개의 데이터를 이용하도록 하였다 (따라서 N은 100의 약수로 하였다)

## 대상
CIFAR-100  
ResNet-50

## Result  
[WandB Result](https://wandb.ai/oso0310/experiment1-2/reports/Experiment-1-2--Vmlldzo1MDA2MjY3)
![image](https://github.com/Chihiro0623/ContinualLearning/blob/main/Experiments/experiment1/experiment1-2/top-1.png)  
![image](https://github.com/Chihiro0623/ContinualLearning/blob/main/Experiments/experiment1/experiment1-2/top-5.png)  

이전의 결과보다는 달성률이 더 높아진 것을 확인할 수 있다  
따라서 혹시나 같은 데이터를 여러번 Duplicate하는 방식으로 결과를 향상시킬 수 있을지 실험해보았다 (WandB의 resnet_50_100_x의 결과들이 바로 이것이다)  

![image](https://github.com/Chihiro0623/ContinualLearning/blob/main/Experiments/experiment1/experiment1-2/top-1of100.png)  

Baseline의 결과가 81.53이므로, 데이터를 복제하지 않았을 때보다는 성능이 저하되었다  
그러나 늘어난 데이터에 맞춘 hyperparameter tuning을 진행한다면 더 좋은 결과가 나올 수도 있다  
적어도 이번 실험에서는 배율이 높아질 수록 성능이 향상되는 것을 확인할 수 있었다  
이는 학습 데이터가 적은 CIFAR에서만 발생하는 현상인지 확인이 필요하다  

## 이후 학습
데이터를 50000개가 아니라 무조건 500개를 사용하도록 수정해본다  
