# Prediction With Uncertainty


The goal of this project is to improve the regression/classification algorithm(s) power.

To this end, during the problem formulation and learning process, we take into account: 

1) Aleatoric uncertainty (the data points variance);
2) Epistemic uncertainty (possible lack of sufficient (training) data);
3) Functional Uncertainty (the initial assumption we made about the data distribution and loss function).


More precisely, every training parameter, ranging from models' weights, loss functions, Etc., can be considered a random variable. Thus we can learn the corresponding distributions.

One of the possible tools is using TensorFlow Probability. See the link below for more:

https://www.tensorflow.org/probability 


Step to process:

1. Implement the two following models and learning processes:
1.a) model the data considering Aleatoric and Epistemic uncertainties;
1.b) model the data considering functional uncertainties;

2. Compare the obtained result with:
1) RNN; (more detail is needed)
2) Plane Variational Gaussian Process (need to think more);
3) Other methods (recommend please)

For the comparison, we will run each of the methods at least five times, and per each run, we will:

A) compute various metrics: including R^score, Mean-relative Absolute errors, MEAPE, Etc, and compute their mean and standard deviations. (See the corresponding W&B project for the list of metrics I have used previously);
B) visual evaluation: plotting the ground truth and predicted values;
C) plot the training and validation loss values.



Link to my notebook warmup with a toy data:

https://github.com/Sorooshi/Prediction_With_Uncertainty


