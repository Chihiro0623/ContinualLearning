 Experiment 1-1
## 가정
학습 과정에서 N개의 Class 중 X개의 Class만을 노출시키면 Top-1 Accuracy가 X/N(%)가 될 것이다

## 대상
CIFAR-100  
ResNet-50

## 결과
[WandB Result](https://wandb.ai/oso0310/experiment1-2/reports/Experiment-1-1--Vmlldzo1MDA2MzIz)
![image](https://github.com/Chihiro0623/ContinualLearning/blob/main/Experiments/experiment1/experiment1-1/top-1.png)  
![image](https://github.com/Chihiro0623/ContinualLearning/blob/main/Experiments/experiment1/experiment1-1/top-5.png)  

top-1 accuracy는 목표 퍼센트가 올라갈 수록 달성률이 떨어지는 경향을 보였다  
top-5 accuracy도 달성률이 떨어지는 경향을 보였으나 대체로 목표를 잘 달성했다  
그러나 Implement 시 미흡한 점이 있었기 때문에 정확한 결과라고 할 수 없다  
