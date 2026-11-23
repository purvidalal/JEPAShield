# JEPA-Shield

**Does noise that makes photos "unlearnable" for one self-supervised method also protect them from others?**

Unlearnable examples add invisible noise to images so models can't learn from them, but they're usually tested only against supervised training. We build protected versions of CIFAR-10, each aimed at one of **SimCLR**, **MAE** or **I-JEPA**, then train ViT-Tiny encoders with all three methods on each version. Comparing linear-probe accuracy on clean test images shows whether the protection transfers between methods, and whether it survives JPEG compression, blur and resizing.

**Stack:** PyTorch · ViT-Tiny · CIFAR-10 · Google Cloud (NVIDIA L4)

**Status:** in progress (COMS 4995 Foundation Model Engineering, Columbia University, Fall 2026)

**Team:** Aditya Kumar Singh · Aniket Gupta · Rakshita Gopal Danee · Purvi Dalal · Tamizhini Venkatesan Kamala
