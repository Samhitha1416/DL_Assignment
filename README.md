# DL_Assignment

##Key Findings

#1. Activation Function

ReLU performs significantly better than Sigmoid.

Sigmoid activation results in poor accuracy, often below 10%.

ReLU achieves much higher validation and test accuracy, reaching 85.98% with momentum.

Sigmoid suffers from the vanishing gradient problem, making deep networks difficult to train.

#2. Initialization Strategy

Xavier initialization consistently improves convergence.

Random initialization struggles, especially with deeper networks.

Xavier initialization maintains proper variance in activations, leading to better training stability.

#3. Optimizer Choice

SGD alone struggles, especially with sigmoid activation.

Momentum and Nesterov Accelerated Gradient (NAG) significantly boost accuracy.

With momentum, validation accuracy reaches 85.98% (Batch Size 16, Xavier, ReLU).

Nesterov momentum shows similar trends and may help in faster convergence.

#4. Batch Size

Smaller batch sizes (16, 32) yield better results.

Provide more stable gradient updates, improving generalization.

Larger batch sizes (64) show slightly lower accuracy.

Less noise in gradient updates may reduce generalization ability.

#5. Learning Rate Considerations

Low learning rate (LR = 0.001) may limit convergence.

A slightly higher learning rate (e.g., 0.005 or 0.01) might speed up training.
