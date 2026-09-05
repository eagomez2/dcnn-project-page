# Official project page: Performance and Complexity Trade-off Optimization of Speech Models During Training
**Esteban Gómez and Tom Bäckström**
Department of Information and Communications Engineering, Aalto University, Espoo, Finland

## Abstract
In speech machine learning, neural network models are typically designed by choosing an architecture with fixed layer sizes and structure. These models are then trained to maximize performance on metrics aligned with the task's objective. While the overall architecture is usually guided by prior knowledge of the task, the sizes of individual layers are often chosen heuristically.

However, this approach does not guarantee an optimal trade-off between performance and computational complexity; consequently, post hoc methods such as weight quantization or model pruning are typically employed to reduce computational cost. This occurs because stochastic gradient descent (SGD) methods can only optimize differentiable functions, while factors influencing computational complexity, such as layer sizes and floating-point operations per second (FLOP/s), are non-differentiable and require modifying the model structure during training.

We propose a reparameterization technique based on feature noise injection that enables joint optimization of performance and computational complexity during training using SGD-based methods. Unlike traditional pruning methods, our approach allows the model size to be dynamically optimized for a target performance-complexity trade-off, without relying on heuristic criteria to select which weights or structures to remove.

We demonstrate the effectiveness of our method through three case studies, including a synthetic example and two practical real-world applications: voice activity detection and audio anti-spoofing. The code related to our work is publicly available to encourage further research.

[[Project page](https://eagomez2.github.io/dcnn-project-page/)] [[Preprint](https://arxiv.org/abs/2601.13704)]

## License
For further details about the license of this tool, please see [LICENSE](LICENSE).

## Acknowledgement
The calculations presented in this publication were carried out using the computer resources of the Aalto University of Science "Science-IT" project.

## Citation
This work has been submitted to the IEEE for possible publication. In the meantime, please cite our preprint:

```bibtex
@misc{gomezbackstrom2026dcnn,
      title={Performance and Complexity Trade-off Optimization of Speech Models During Training}, 
      author={Esteban Gómez and Tom Backström},
      year={2026},
      eprint={2601.13704},
      archivePrefix={arXiv},
      primaryClass={cs.SD},
      url={https://arxiv.org/abs/2601.13704}, 
}
```
