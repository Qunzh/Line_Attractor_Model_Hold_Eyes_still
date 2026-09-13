# Line Attractor based on Linear Network Model + Readout Network

## Overview
Reproduction of Line Attractor with Linear Network Model + Readout Network for Working Memory for Eye Angular Position based on Seung et al.(1996) 

Linear Network Model
```math
\tau_s \dfrac{du_i}{dt} = -u_i + \sum^N_{j = 1}T_{ij}v_j + h_i \space (1)
```
```math
v_i \approx g_iu_i + v^p_i
```
Readout Network
```math
\tau_r \dfrac{dr_m}{dt} = -r_m + \sum^N_{j = 1}C_{mj}v_j + b_m \space (1)
```


### Explanation for the Model
This is the linear neural network 

### Significance of Model
