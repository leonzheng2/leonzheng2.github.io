---
layout: archive
title: "Code"
permalink: /code/
author_profile: true
---
The code for most papers is available on <span style="color:blue">[Github](https://github.com/leonzheng2)</span>.


# Measuring progress in diffusion language model pretraining

![speedrun-dlm](/files/speedrun-dlm.png)

**Code**: available <span style="color:blue">[here](https://github.com/agonon/speedrun-dlm)</span>.

If you use this code, please cite the following paper: "Measuring progress in diffusion language model pretraining", A. Gonon, A. Müller, L. Zheng, C. Lalanne, Z. Shen, Y.-P. Hsieh, A. Bardou, N. Boumal, *NeurIPS 2026 Workshop: Beyond Next Token Prediction: Diffusion and Flow Models for Next-Generation Decoding*, 2026.

<span style="color:blue">[Link to paper](https://openreview.net/forum?id=WLNBGbEQnV)</span>.

**Description**: A speedrun benchmark for diffusion language models (DLMs): train a DLM on FineWeb as fast as possible, until it reaches a fixed HellaSwag target accuracy. The model (a 170M-parameter DDiT backbone), the data and the hardware are fixed, so submissions are comparable. The repository includes re-implementations of common diffusion training recipes and a leaderboard of training times.


# Fast inference with Kronecker-sparse matrices

![ksmm](/files/ksmm.png)

**Code**: available <span style="color:blue">[here](https://github.com/PascalCarrivain/ksmm)</span>.

If you use this code, please cite the following paper: "Fast inference with Kronecker-sparse matrices", A. Gonon, L. Zheng, P. Carrivain, Q. T. Le, *International Conference on Machine Learning* (ICML), PMLR 267:20075-20102, 2025.

<span style="color:blue">[Link to paper](https://openreview.net/forum?id=RuMfpz8bTw)</span>.

**Abstract**: Kronecker-sparse (KS) matrices—whose supports are Kronecker products of identity and all-ones blocks—underpin the structure of Butterfly and Monarch matrices and offer the promise of more efficient models. However, existing GPU kernels for KS matrix multiplication suffer from high data movement costs, with up to 50% of time spent on memory-bound tensor permutations. We propose a fused, output-stationary GPU kernel that eliminates these overheads, reducing global memory traffic threefold. Across 600 KS patterns, our kernel achieves in FP32 a median speedup of x1.4 and lowers energy consumption by 15%. A simple heuristic based on KS pattern parameters predicts when our method outperforms existing ones. We release all code at github.com/PascalCarrivain/ksmm, including a PyTorch-compatible KSLinear layer, and demonstrate in FP32 end-to-end latency reductions of up to 22% in ViT-S/16 and 16% in GPT-2 medium.


# Self-supervised learning with rotation-invariant kernels

![sfrik](/files/sfrik.png)

**Code**: available <span style="color:blue">[here](https://github.com/valeoai/sfrik)</span>.

If you use this toolbox, please cite the following paper: "Self-supervised learning with rotation-invariant kernels", L. Zheng, G. Puy, E. Riccietti, P. Pérez, R. Gribonval, *International Conference on Learning Representations* (ICLR), 2023.

<span style="color:blue">[Link to paper](https://arxiv.org/abs/2208.00789)</span>.

**Abstract**: We introduce a regularization loss based on kernel mean embeddings with rotation-invariant kernels on the hypersphere (also known as dot-product kernels) for self-supervised learning of image representations. Besides being fully competitive with the state of the art, our method significantly reduces time and memory complexity for self-supervised training, making it implementable for very large embedding dimensions on existing devices and more easily adjustable than previous methods to settings with limited resources. Our work follows the major paradigm where the model learns to be invariant to some predefined image transformations (cropping, blurring, color jittering, etc.), while avoiding a degenerate solution by regularizing the embedding distribution. Our particular contribution is to propose a loss family promoting the embedding distribution to be close to the uniform distribution on the hypersphere, with respect to the maximum mean discrepancy pseudometric. We demonstrate that this family encompasses several regularizers of former methods, including uniformity-based and information-maximization methods, which are variants of our flexible regularization loss with different kernels. Beyond its practical consequences for state-of-the-art self-supervised learning with limited resources, the proposed generic regularization approach opens perspectives to leverage more widely the literature on kernel methods in order to improve self-supervised learning methods.

# Butterfly sparse matrix factorization

![butterfly](/files/butterfly.png)

## Efficient identification of butterfly sparse matrix factorization.

**Code**: available <span style="color:blue">[here](https://github.com/leonzheng2/efficient-butterfly)</span>.

If you use this toolbox, please cite the following paper: "Efficient Identification of Butterfly Sparse Matrix Factorizations", L. Zheng, E. Riccietti, R. Gribonval, *SIAM Journal on Mathematics of Data Science*, 5(1), 22-49., 2023.

<span style="color:blue">[Link to paper](https://arxiv.org/abs/2110.01230)</span>.

**Abstract**: Fast transforms correspond to factorizations of the form $Z=X^{(1)} ... X^{(J)}$, where each factor $X^{(\ell)}$ is sparse and possibly structured. This paper investigates essential uniqueness of such factorizations, i.e., uniqueness up to unavoidable scaling ambiguities. Our main contribution is to prove that any N×N matrix having the so-called butterfly structure admits an essentially unique factorization into J butterfly factors (where $N=2^J$), and that the factors can be recovered by a hierarchical factorization method, which consists in recursively factorizing the considered matrix into two factors. This hierarchical identifiability property relies on a simple identifiability condition in the two-layer and fixed-support setting. This approach contrasts with existing ones that fit the product of butterfly factors to a given matrix via gradient descent. The proposed method can be applied in particular to retrieve the factorization of the Hadamard or the discrete Fourier transform matrices of size $N=2^J$. Computing such factorizations costs $O(N^2)$, which is of the order of dense matrix-vector multiplication, while the obtained factorizations enable fast $O(N \log N)$ matrix-vector multiplications and have the potential to be applied to compress deep neural networks.


## Fast learning of fast transforms, with guarantees.

**Code**: available <span style="color:blue">[here](https://github.com/leonzheng2/butterfly)</span>.

If you use this toolbox, please cite the following paper: "Fast learning of fast transforms, with guarantees", Q. T. Le, L. Zheng, E. Riccietti, R. Gribonval, *IEEE International Conference on Acoustics, Speech and Signal Processing* (ICASSP), 2022.

<span style="color:blue">[Link to paper](https://ieeexplore.ieee.org/abstract/document/9747791)</span>.

**Abstract**: Approximating a matrix by a product of few sparse factors whose supports possess the butterfly structure, which is common to many fast transforms, is key to learn fast transforms and speed up algorithms for inverse problems. We introduce a hierarchical approach that recursively factorizes the considered matrix into two factors. Using recent advances on the well-posedness and tractability of the two-factor fixed- support sparse matrix factorization problem, the proposed algorithm is endowed with exact recovery guarantees. Experiments show that speed and accuracy of the factorization can be jointly improved by several orders of magnitude, compared to gradient-based optimization methods.
