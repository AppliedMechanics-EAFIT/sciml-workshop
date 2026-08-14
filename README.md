# PINNs práctico: resolviendo problemas directos e inversos con redes neuronales

![GitHub](https://img.shields.io/github/license/AppliedMechanics-EAFIT/sciml-workshop)
[![License: CC BY 4.0](https://img.shields.io/badge/License-CC_BY_4.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)
[![Abrir en Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/AppliedMechanics-EAFIT/sciml-workshop/HEAD)
[![Abrir en Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/AppliedMechanics-EAFIT/sciml-workshop)

Este repositorio contiene material sobre redes neuronales informadas por la física
(PINNs, del inglés Physics-Informed Neural Newtorks) y está pensado para un taller
en el marco del SciML Medellín 2026 realizado en la Universidad EAFIT.

## Contenido

 1. [Motivación](#motivación)
 2. [Contenido](#contenido-del-minicurso)
 2. [Referencias](#material-relacionado-y-algunas-referencias)
 3. [Licencia](#licencia)
 4. [Agradecimientos](#agradecimientos)

## Motivación

En los últimos años, las redes neuronales profundas se han convertido en herramientas fundamentales para la modelación y el análisis de datos complejos en espacios de alta dimensionalidad. No obstante, estas técnicas suelen requerir grandes volúmenes de datos para ajustar sus numerosos parámetros, lo cual no siempre es viable en situaciones donde la disponibilidad de datos es limitada. Para abordar este desafío, se han desarrollado métodos innovadores, como las Redes Neuronales Informadas por Física (PINNs), que combinan el aprendizaje profundo con la información física del problema a resolver. Basadas en el teorema de aproximación universal, estas redes son capaces de aproximar funciones no lineales complejas bajo ciertas arquitecturas [(Hornik, 1991)](https://www.sciencedirect.com/science/article/pii/089360809190009T?via%3Dihub), [(Barron, 1993)](https://ieeexplore.ieee.org/document/256500), [(Villota, 2019)](https://investigacion.unirioja.es/documentos/5fbf7e47299952682503c2fa/). Adicionalmente, el uso de diferenciación automática [(Baydin *et al.*, 2018)](https://arxiv.org/abs/1502.05767) permite que las PINNs resuelvan modelos físicos complejos sin la necesidad de grandes cantidades de datos. Esta integración de información adicional facilita la optimización del modelo, permitiendo un mayor nivel de precisión y robustez en aplicaciones donde los datos disponibles son escasos [(Raissi *et al.*, 2019)](https://www.sciencedirect.com/science/article/pii/S0021999118307125), [(Karniadakis *et al.*, 2021)](https://www.nature.com/articles/s42254-021-00314-5).

## Contenido del minicurso

<center>

| Actividad    |  Link| 
| ------------- | --------- | 
| Taller teórico: conceptos básicos y aplicaciones | [Link](https://github.com/dortiz5/ihealth-pinns-mini-course/blob/main/slides/taller_teorico.pdf) | 
| Lect 1 – Introducción a las PINNs: sistema masa–resorte amortiguado  | [![Activity 1](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/AppliedMechanics-EAFIT/sciml-workshop/blob/main/notebooks/Lect%201%20-%20PINN%20Mass%20-%20spring-%20damper.ipynb) |
| Lect 2 – ANN vs PINNs: modelo del péndulo no lineal | [![Activity 2](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/AppliedMechanics-EAFIT/sciml-workshop/blob/main/notebooks/Lect%202%20-%20ANN%20Vs%20PINN%20-%20pendulum.ipynb) |
| Lect 3 – PINNs 2D: difusión directa |  [![Activity 3](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/AppliedMechanics-EAFIT/sciml-workshop/blob/main/notebooks/Lect%203%20-%202D%20PINNS%20diffusion%20-%20direct.ipynb) |
| Lect 4 – PINNs 2D: difusión inversa | [![Activity 4](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/AppliedMechanics-EAFIT/sciml-workshop/blob/main/notebooks/Lect%204%20-%202D%20PINNS%20diffusion%20-%20inverse.ipynb) |
| Lect 5 – Temas avanzados en PINNS | TBA |

</center>


## Material relacionado y algunas referencias:


- Redes Neuronales Artificiales: [Interesante serie de vídeos de 3Blue1Brown sobre redes neuronales y aprendizaje automático](https://www.3blue1brown.com/topics/neural-networks)

- Diferenciación automática. Aquí encontrará 3 enlaces sobre la diferenciación automática y los números duales: [link 1](https://thenumb.at/Autodiff/), [link 2](https://blog.demofox.org/2014/12/30/dual-numbers-automatic-differentiation/), [link 3](https://en.wikipedia.org/wiki/Dual_number). Además, aquí puedes encontrar un  [tutorial](https://pytorch.org/tutorials/beginner/blitz/autograd_tutorial.html#a-gentle-introduction-to-torch-autograd) en PyTorch

- [Redes neuronales basadas en la física para visión por ordenador e imágenes médicas [1].](https://collab.dvb.bayern/display/TUMdlma/Physics+Informed+Neural+Network+for+Computer+Vision+and+Medical+Imaging)

- Ben Moseley [blog personal](https://benmoseley.blog/)


Existen muchos artículos científicos relacionados con PINNs. A continuación,
compartimos algunos que pueden servir de punto de partida:

- Raissi, Maziar, Paris Perdikaris, and George E. Karniadakis.
  ["Physics-informed neural networks: A deep learning framework for solving
  forward and inverse problems involving nonlinear partial differential
  equations."](https://www.sciencedirect.com/science/article/pii/S0021999118307125)
  Journal of Computational physics 378 (2019): 686-707.

- Karniadakis, George Em, et al.
  ["Physics-informed machine learning."](https://doi.org/10.1038/s42254-021-00314-5)
  Nature Reviews Physics 3.6 (2021): 422-440.

- Chuang, Pi-Yueh, and Lorena A. Barba.
  ["Predictive limitations of physics-informed neural networks in vortex shedding."]
  (https://arxiv.org/abs/2306.00230) arXiv preprint arXiv:2306.00230 (2023).

- Krishnapriyan, Aditi, et al. ["Characterizing possible failure modes
  in physics-informed neural networks."](https://arxiv.org/abs/2109.01050)
  Advances in Neural Information Processing Systems 34 (2021): 26548-26560.

- Wang, Sifan, et al. ["An expert's guide to training physics-informed neural networks."](https://arxiv.org/abs/2308.08468)
arXiv preprint arXiv:2308.08468 (2023).

- Jara, S., Sotelo, J., Ortiz-Puerta, D., Estévez, P. A., Uribe, S.,
  Chabert, S., & Salas, R. (2025). Physics-Informed Neural Network for Modeling
  the Pulmonary Artery Blood Pressure from Magnetic Resonance Images: A
  Reduced-Order Navier–Stokes Model. Biomedicines, 13(9), 2058. DOI:
  [10.3390/biomedicines13092058](https://doi.org/10.3390/biomedicines13092058).

- Olivares, M. B., Castrillón, J. D. A., & Muñoz, D. A. (2026). Physics-Informed
  Deep Learning for Industrial Processes: Time-Discrete VPINNs for heat conduction.
  arXiv preprint arXiv: [2603.04711](https://arxiv.org/abs/2603.04711).

- Rincón-Cardeño, Ó., Pérez-Bernal, G., Montoya-Noguera, S., & Guarín-Zapata, N.
  (2026). A Scoping Review of Physics Informed Machine Learning for Wave
  Propagation Modeling in Seismology. arXiv preprint arXiv:[2607.00178](https://arxiv.org/abs/2607.00178).


## Licencia

Todo el código está bajo licencia MIT y el contenido bajo licencia Creative Commons Attribute.

El contenido de este repositorio está bajo licencia bajo la
[Licencia Creative Commons Attribution 4.0](http://choosealicense.com/licenses/cc-by-4.0/),
y el código fuente que acompaña al contenido tiene 
[Licencia MIT](https://opensource.org/licenses/mit-license.php).


## Agradecimientos

Este taller se pudo llevar a cabo gracias a la colaboración de las siguientes
instituciones:

- Universidad EAFIT (programa 12330032023);
- Universidad Nacional de Colombia – Sede Medellín;
- Institución Universitaria Pascual Bravo;
- Universidad de Valparaíso – Chile;
- Instituto Milenio – iHealth (Programa Iniciativa Científica Milenio ICN2021_004); y
- Agencia Nacional de Investigación y Desarrollo (Chile) – ANID (proyecto Fondecyt de posdoctorado 3250439).

