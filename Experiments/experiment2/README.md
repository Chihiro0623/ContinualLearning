# Experiment 1-2  
## 가정
학습 과정에서 N개의 Class 중 X개의 Class만을 노출시키면 Top-1 Accuracy가 X/N(%)가 될 것이다  
[이전의 실험](https://github.com/Chihiro0623/ContinualLearning/tree/main/Experiments/experiment1)에서는 총 50000개의 데이터 중 N개의 Class에 해당하는 데이터, 즉 N*500개의 데이터만을 이용했으나, 이번 실험에는 데이터를 중복시키는 방법으로 N의 수와 관계없이 50000개의 데이터를 이용하도록 하였다 (따라서 N은 100의 약수로 하였다)

## 대상
CIFAR-100  
ResNet-50

## Result  
[WandB Result](https://api.wandb.ai/links/oso0310/k1f1i0tn)
![image](https://github.com/Chihiro0623/ContinualLearning/Experiments/experiment1/Result.png)  
