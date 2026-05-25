# ai-hw-spring-2026-aa
Assignment #7.1: Attack MNIST Recognition

The results show that larger epsilon values lead to stronger attacks. FGSM has the lowest ASR because it uses only one gradient step, while PGD and Momentum I-FGSM are much stronger because they update the adversarial examples iteratively. At ϵ=0.3, PGD and Momentum I-FGSM almost completely fool the model, even though the model has a clean test accuracy of 99.28%. This shows that high accuracy on clean images does not guarantee robustness against adversarial examples.
