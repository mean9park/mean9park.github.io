---
layout: single
title: "Matrix Decomposition, SVD (Singular Vector Decomposition)"
description: SVD(Singular Vector Decomposition)
date: "2022-04-18 11:30:00 +0900"
last_modified_at: "2022-04-18 21:30:00 +0900"
tags: ["Linear Algebra", "Matrix"]
---

---

# SVD (Singular Vector Decomposition)

> Decomposition
---

<img src="https://latex.codecogs.com/svg.image?\LARGE&space;A^{m\times&space;n}&space;=&space;U&space;\Sigma&space;V^{T}" title="https://latex.codecogs.com/svg.image?\LARGE A^{m\times n} = U \Sigma V^{T}" />

<img src="https://latex.codecogs.com/svg.image?\LARGE&space;U^{m\times&space;m}" title="https://latex.codecogs.com/svg.image?\LARGE U^{m\times m}" />
= Left Singular Vector (Eigendecompotision of
<img src="https://latex.codecogs.com/svg.image?\large&space;AA^{T}" title="https://latex.codecogs.com/svg.image?\large AA^{T}" />
)
<img src="https://latex.codecogs.com/svg.image?\LARGE&space;V^{n\times&space;n}" title="https://latex.codecogs.com/svg.image?\LARGE V^{n\times n}" />
 = Right Singular Vector (Eigendecomposition of 
<img src="https://latex.codecogs.com/svg.image?\large&space;A^{T}A" title="https://latex.codecogs.com/svg.image?\large A^{T}A" />
)


> Pytorch Implementation
---

Let's see it actually works anyway, here's a 5X5 matrix.
```python
import numpy as np
from numpy.linalg import svd

a = np.random.rand(5, 5)
np.round(a, 4)
U, Sigma, V = np.linalg.svd(a)
```
<p align="center">
  <img src="../assets/images/SVD_array.png" alt="svd array" width="500"/>
</p>
```python
U, Sigma, V = svd(a)
```

```python
print('U matrix : ', np,round(U, 4))
print('Sigma : ', np,round(Sigma, 4))
print('V transpose matrix : ', np,round(V, 4))
```
<p align="center">
  <img src="../assets/images/decomposition.png" alt="decomposition components" width="500"/>
</p>
```python
Sigma_mat = np.diag(Sigma)
a_reconstructed = np.matmul(np.matmul(U, Sigma), V)
print(a_reconstructed)
```
<p align="center">
  <img src="../assets/images/reconstructed_SVD_array.png" alt="reconstructed array" width="500"/>
</p>

good <br>
and it's `one line code` let's see

[Google](https://google.com)

![come on crow~!](../assets/images/crow.png)

Below is APPLE crow

[![click on crow~!](../assets/images/crow.png)](https://apple.com)
