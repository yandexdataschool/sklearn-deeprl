### Deep reinforcement learning. In scikit-learn. In less than 50 effective lines.
Dive-in button: [![Binder](http://mybinder.org/badge.svg)](http://mybinder.org:/repo/yandexdataschool/sklearn-deeprl)

Currently both demos are vanilla crossentropy(CE) method for policy approximated by a neural network.
For RL, it boild down to
Repeat:
* Generate N games
* Take M best
* Fit to those M best samples

The CE is a very general approach for approximate estimation and maximization tasks, you can read about it [here](https://people.smp.uq.edu.au/DirkKroese/ps/eormsCE.pdf). For reinforcement learning, we use the optimization version, basically trying to fit agent to generating games where reward is high. More on that [here](http://www.aaai.org/Papers/ICML/2003/ICML03-068.pdf).

While this approach falls flat in some cases and it takes black magic to make it work with infinite MDPs or long session lengths, it still works unreasonably well in most cases. One more awesome trait is that it extendds effortlessly to policy approximation (e.g. deep RL), partially observable MDPs and all kinds of weird stuff you see in the wild.

If you want something heavier, take a look at [agentnet](https://github.com/yandexdataschool/AgentNet).

