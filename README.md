# PUGNet
The official implement of 《Progressive Uncertainty Guided Network for Binary Segmentation》

# Performance Comparison on COD Datasets

| Baseline       | Backbone     | CAMO (250 images) % |                |                 |                | COD10K (2026 images) % |                 |                  |                 | NC4K (4121 images) % |                |                  |                  |
|----------------|--------------|---------------------|----------------|-----------------|----------------|----------------------|-----------------|------------------|-----------------|---------------------|----------------|------------------|------------------|
|                |              | $S_{\alpha}\uparrow$ | $E_{\phi}\uparrow$ | $F^w_{\beta}\uparrow$ | $M\downarrow$ | $S_{\alpha}\uparrow$ | $E_{\phi}\uparrow$ | $F^w_{\beta}\uparrow$ | $M\downarrow$ | $S_{\alpha}\uparrow$ | $E_{\phi}\uparrow$ | $F^w_{\beta}\uparrow$ | $M\downarrow$ |
|----------------|--------------|---------------------|----------------|-----------------|----------------|----------------------|-----------------|------------------|-----------------|---------------------|----------------|------------------|------------------|
| SINet          | ResNet-50    | 75.1                | 77.1           | 60.6            | 10.0           | 77.1                 | 80.6            | 55.1             | 5.1             | 80.8                | 87.1           | 73.8             | 5.8              |
| UGTR$^{*}$     | ResNet-50    | 78.4                | 82.1           | 68.3            | 8.6            | 81.7                 | 85.2            | 66.5             | 3.6             | 83.9                | 87.4           | 75.5             | 5.2              |
| MGL v2         | ResNet-50    | 77.4                | 84.8           | 68.4            | 8.5            | 81.3                 | 88.2            | 68.2             | 3.4             | 83.1                | 89.2           | 75.1             | 5.1              |
| PFNet          | ResNet-50    | 78.2                | 84.2           | 69.5            | 8.5            | 80.0                 | 87.7            | 66.0             | 4.0             | 82.9                | 88.6           | 74.7             | 5.3              |
| SINet v2       | Res2Net-50   | 82.0                | 88.2           | 74.3            | 7.0            | 81.5                 | 88.7            | 68.0             | 3.7             | 84.7                | 90.3           | 76.7             | 4.8              |
| CA-Net$^{*}$   | ResNet-50    | 80.7                | 86.6           | 76.7            | 7.5            | 83.2                 | 89.0            | 74.5             | 3.2             | 85.7                | 89.9           | 81.7             | 4.4              |
| UR-COD$^{*}$   | Res2Net-50   | 81.4                | 89.1           | 75.8            | 6.7            | 81.6                 | 90.3            | 70.8             | 3.3             | 84.4                | 91.0           | 78.7             | 4.5              |
| ZoomNet        | ResNet-50    | 82.0                | 89.2           | 75.2            | 6.6            | 83.8                 | 91.1            | 72.9             | 2.9             | 85.3                | 91.2           | 78.4             | 4.3              |
| FDNet          | Res2Net-50   | 84.4                | 89.8           | 77.8            | 6.2            | 83.7                 | 91.8            | 73.1             | 3.0             | -                   | -              | -                 | -                |
| FEDER          | Res2Net-50   | 83.6                | 89.7           | 80.7            | 6.6            | 84.4                 | 91.1            | 74.8             | 2.9             | 86.2                | 91.3           | 82.4             | 4.2              |
| DTIT           | Mit-b5       | 85.7                | 91.6           | 79.6            | 5.0            | 82.4                 | 89.6            | 69.5             | 3.4             | 86.3                | 91.7           | 79.2             | 4.1              |
| HitNet         | PVT-v2-b2    | 84.4                | 90.2           | 80.1            | 5.7            | **86.8**             | 93.2       | **79.8**         | **2.4**         | 87.0                | 92.1           | 82.5             | 3.9              |
| FSPNet         | ViT          | 85.6                | 89.9           | 79.9            | 5.0            | 85.1                 | 89.5            | 73.5             | 2.6             | **87.9**            | 91.5           | 81.6             | **3.5**          |
| UEDG$^{*}$     | PVT-v2-b2    | 86.8            | 92.2      | 81.9         | 4.8        | 85.8                 | 92.4            | 76.6             | 2.5             | **88.1**            | **92.8**       | **82.9**         | **3.5**          |
| **PUGNet$^{*}$** | PVT-v2-b2 | **87.0**            | **93.8**       | **84.7**         | **4.2**        | 86.1                 | **93.5**        | 79.2             | **
