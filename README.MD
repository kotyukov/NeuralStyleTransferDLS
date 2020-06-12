# Neural Style Transfer study case for DLS MIPT

This is NST-algorithm implementation inspired by paper "A Neural Algorithm of Artistic Style", Gatys, Ecker, Bethge. [1508.06576](https://arxiv.org/pdf/1508.06576.pdf "1508.06576")

Original Neural Style Transfer code by Leon Gatys:
https://github.com/leongatys/PytorchNeuralStyleTransfer



### The loss function
we minimise is

$$L_{total}(\vec{p},\vec{a},\vec{x})$$ = $$\alpha$$ $$L_{content}(\vec{p},\vec{x})$$ + $$\beta$$ $$L_{style}(\vec{a},\vec{x})$$

where $$\vec{a}$$ is style image, $$\vec{p}$$ is content image, $$\vec{x}$$ is generated (output) image and
$$\alpha$$ and $$\beta$$ are the weighting factors for content and style.

![](https://raw.githubusercontent.com/kotyukov/NeuralStyleTransferDLS/master/data/losses.png)

### Transfer two styles (fusion)

![](https://raw.githubusercontent.com/kotyukov/NeuralStyleTransferDLS/master/data/fusion.png)

### Transfer two styles (naive split)

![](https://raw.githubusercontent.com/kotyukov/NeuralStyleTransferDLS/master/data/split.png)

### Layer-sets comparison

![](https://raw.githubusercontent.com/kotyukov/NeuralStyleTransferDLS/master/data/layers.png)

### Pooling type comparison

![](https://raw.githubusercontent.com/kotyukov/NeuralStyleTransferDLS/master/data/pooling.png)