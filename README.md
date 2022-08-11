# MBPO with [ReLAx](https://github.com/nslyubaykin/relax)
Example MBPO-SAC implementation with [ReLAx](https://github.com/nslyubaykin/relax)

This repository contains an implementation of MBPO algorithm for SAC actor with [ReLAx](https://github.com/nslyubaykin/relax) package.

The performance versus vanilla SAC is measured by averaging learning curves (for separate evaluation environment) over 4 experiments with random environment seeds.

The results are summarized in the following plot (MBPO is run only for 175k envsteps to save training time):

![mbpo_training](https://github.com/nslyubaykin/relax_mbpo_example/blob/master/mbpo_training.png)

The only difference in hyper-parameters settings between MBPO-SAC and vanilla SAC is the presence of model based acceleration. 
We can see a substantial advantage of MBPO in terms of training speed by looking at the averaged curves.

__Resulting Policy__

https://user-images.githubusercontent.com/67604207/184105444-bcdad145-1dde-4c9f-a8fd-f384a14e8f90.mp4
