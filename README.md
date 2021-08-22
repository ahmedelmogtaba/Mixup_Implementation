# Mixup_Implementation

# First Experiment (CIFAR10)

| Model  | Epoch | Weight_decay| Learning rate | Validation accuracy |
| ------------- | ------------- |--------------------|--------------------|------------------------------|
| ERM (Resnet18)  | 200 |   1e-4                         |    0.1                 |      95.79                |
| Mix_up (Resnet18) | 200 |        1e-4                   |        0.1            |        94.63              |



# Graphs

![im_1](https://user-images.githubusercontent.com/45710249/130177946-eb8654e6-038f-4532-b322-606bd5dc8c9e.png)

![im_2](https://user-images.githubusercontent.com/45710249/130177972-f1e3e1bc-b2eb-488f-8287-0ed99f3ff78a.png)

# Second Experiment (Robustness to Adversarial Examples)

 Note that the architecture used in the paper in this task is Resnet101 and I used Resnet18 , also the dataset is Imagenet and I used CIFAR10.

| Model  | Experiment | My Result| Paper Result |
| ------------- | ------------- |-------------------|------------------------------|
| Mix_up (Resnet18)  | white box attack |     49.25       |      75.2               |
| ERM (Resnet18) | white box attack |    53.7          |       90.7        |
|    Mix_up (Resnet18)            |        black box attack          |        49.76             |        46.0            |
|       ERM (Resnet18)          |      black box attack           |        55.07        |      57.0             | 


# Third Experiment (Tabular Data) :
|Dataset| Model  | Epoch |My Result | Paper Result |
|------------| ------------- | ------------- |--------------------|------------------------------|
|Abalone DataSet| ERM (MLP)  | 10               |     68.5                |      74.0               |
|Abalone Dataset| Mix_up (MLP) | 10                |        68.1         |        73.6            |
|Iris Dataset |ERM (MLP) | 10 | 86.6 | 78.7 |
|Iris Dataset| Mix_up (MLP) | 10   | 89.9  | 82.7 |
