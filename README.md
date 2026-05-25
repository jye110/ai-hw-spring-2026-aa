# ai-hw-spring-2026-aa
Test Accuracy: 99.28%

Epsilon = 0.05
FGSM ASR:     0.0321
PGD ASR:      0.0504
MI-FGSM ASR:  0.0492

Epsilon = 0.1
FGSM ASR:     0.1354
PGD ASR:      0.3081
MI-FGSM ASR:  0.2882

Epsilon = 0.2
FGSM ASR:     0.6714
PGD ASR:      0.9590
MI-FGSM ASR:  0.9525

Epsilon = 0.3
FGSM ASR:     0.8708
PGD ASR:      0.9998
MI-FGSM ASR:  0.9995

The results show that larger epsilon values lead to stronger attacks. FGSM has the lowest ASR because it uses only one gradient step, while PGD and Momentum I-FGSM are much stronger because they update the adversarial examples iteratively. At ϵ=0.3, PGD and Momentum I-FGSM almost completely fool the model, even though the model has a clean test accuracy of 99.28%. This shows that high accuracy on clean images does not guarantee robustness against adversarial examples.
