# ALL-PET
Currently, the construction of large-scale foundation models in the field of PET imaging faces two core bottlenecks: first, data scarcity. Affected by privacy and ethical restrictions, as well as the high cost of expert annotations, it is difficult to obtain high-quality annotated PET data, and the original projection data is complex and scarce; second, high demand for computing resources. Most existing medical foundation models rely on hundreds of millions of parameters and multi-GPU clusters, making them difficult to deploy in low-resource scenarios such as primary hospitals. In addition, most models operate in the image domain and discard the physical priors (such as attenuation effects and angle dependence) in the projection domain (sinogram space), resulting in outputs that may lack physical consistency and affect diagnostic reliability.

To address this, the research team proposed ALL-PET — the first PET foundation model that operates in the projection domain, with low resource requirements (24GB memory on a single GPU) and few samples (only 500 sinograms per task). It aims to directly capture physical priors from sinograms, balancing performance, interpretability, and clinical adaptability.
![]()

## Fig. 1. Overview of the ALL-PET foundation model and traininginference pipeline.
![](./Fig. 1. Overview of the ALL-PET foundation model and traininginference pipeline..png)  

# Generation of PET Projection Domain
<table>
  <tr>
    <td><img src="https://github.com/yqx7150/ALL-PET/blob/main/PET_gif/gif%20(32).gif" alt="GIF 1" style="width:300px;height:300px;"></td>
    <td><img src="https://github.com/yqx7150/ALL-PET/blob/main/PET_gif/gif%20(33).gif" alt="GIF 2" style="width:300px;height:300px;"></td>
    <td><img src="https://github.com/yqx7150/ALL-PET/blob/main/PET_gif/gif%20(35).gif" alt="GIF 3" style="width:300px;height:300px;"></td>
  </tr>
  <tr>
    <td><img src="https://github.com/yqx7150/ALL-PET/blob/main/PET_gif/gif%20(36).gif" alt="GIF 4" style="width:300px;height:300px;"></td>
    <td><img src="https://github.com/yqx7150/ALL-PET/blob/main/PET_gif/gif%20(37).gif" alt="GIF 5" style="width:300px;height:300px;"></td>
    <td><img src="https://github.com/yqx7150/ALL-PET/blob/main/PET_gif/gif%20(38).gif" alt="GIF 6" style="width:300px;height:300px;"></td>
  </tr>
</table>

# Generation of PET dominated by the projection domain
<table>  
  <tr>
    # Generation of PET_body images
    <td><img src="https://github.com/yqx7150/ALL-PET/blob/main/PET_body/0.png" alt="GIF 1" style="width:300px;height:300px;"></td>
    <td><img src="https://github.com/yqx7150/ALL-PET/blob/main/PET_body/89.png" alt="GIF 2" style="width:300px;height:300px;"></td>
    <td><img src="https://github.com/yqx7150/ALL-PET/blob/main/PET_body/97.png" alt="GIF 3" style="width:300px;height:300px;"></td>
  </tr>
  
</table>


