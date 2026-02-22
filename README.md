# Synthetic Image Detector

This project explores the growing challenge of detecting AI generated synthetic images in a world where generative models are becoming increasingly realistic. We followed a Build, Break, Improve framework to evaluate both the performance and robustness of a synthetic image detector. First, we fine tuned a pretrained ResNet18 model on the CIFAKE dataset to classify real and synthetic images. The model achieved strong performance across accuracy, precision, recall, and F1 score. To better understand its decision making process, we used Grad CAM and saliency maps, which revealed that the model relied heavily on fine texture patterns and high frequency artifacts.

Next, we tested the robustness of the detector using the Fast Gradient Sign Method. Small, visually imperceptible perturbations significantly reduced confidence scores and in several cases flipped predictions from fake to real. This demonstrated that high classification accuracy does not guarantee robustness.

Based on these findings, we propose adversarial training as a concrete improvement strategy to strengthen the model against such vulnerabilities. This work highlights the importance of evaluating AI systems not only for performance but also for resilience in adversarial settings.

demo explanation video drive link: https://drive.google.com/drive/folders/1BWd4Kuo-tlgTMiyLVQQT1GgCYnT2borg?usp=sharing
