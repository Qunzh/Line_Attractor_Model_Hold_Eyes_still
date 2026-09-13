# Line Attractor based on Linear Network Model + Readout Network

## Overview
Reproduction of Line Attractor with Linear Network Model + Readout Network for Working Memory for Eye Angular Position based on Seung et al.(1996) 

Linear Network Model
```math
\tau_s \dfrac{du_i}{dt} = -u_i + \sum^N_{j = 1}T_{ij}v_j + h_i \space (1)
```
```math
v_i \approx g_iu_i + v^p_i \space (2)
```
Readout Network
```math
\tau_r \dfrac{dr_m}{dt} = -r_m + \sum^N_{j = 1}C_{mj}v_j + b_m \space (3)
```


### Explanation for the Models
The memory of eye position is modeled by two network: the memory network and the readout network. The memory networks is based on Linear Network Model. The Linear Network Model is composed by two equations. Equation (1) describes the total synaptic current input $u_i$ which each neuron $i$ inside memory network receives from recurrent and feedforward connection. The recurrent connection is described by $\sum^N_{j = 1}T_{ij}v_j$, which sum up all the recurrent connection  which neuron $i$ receives from other neuron j inside memory work with synaptic connection $T_{ij}$. The feedforward connection is described by $h_i$ , which is information about the position of the head, and is a constant term when the head position is still (an assumption of the model). Equation (2) describes the firing rate $v_i$ of neuron $i$, which is a linear sum of multiple of synaptic conductance $g_i$ and synaptic current $u_i$ and spontaneous pacemaker activity $v^p_i$. 

### Significance of Model
