# CNN CIFAR10 gradcam cutout
Improving generalization and reducing overfitting using cutout for better generalization

## References

- https://arxiv.org/pdf/1708.04552.pdf


## Approach

- Build CNN Model using Batch Normalization, Dropout
- Relu activations for the layers; Softmax for the output layer
- Paramters < 1/2 Million
- Enabled GradCam class activation
- Superimposed the generated heatmap on the original image to understand class activation
- Run 50 epochs
- Option1 - Enabled without cutout
- Option2 - Enabled with cutout

## Observations

- Without Cutout : 81.44 % test accuracy on CIFAR
- With Cutout    : 83.98 % test accuracy on CIFAR

