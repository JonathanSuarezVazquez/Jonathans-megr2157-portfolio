# A7 – [FEA on Bracket]

## Objective

The objective for this assignment is to optimize the design of our bracket and link from the previous assignment #5. We will use finite element analysis to help assist us with modifications to improve our bracket. The FEA will give us data on the strength, stiffness, and safety factor of our bracket, using that date we will try to make it more lightweight. We are also tasked with documenting our processes and decision choices. 

## Analyze

## Bracket
### First Iteration

To begin I opened solidworks and opened my bracket, I then hit simulation and created a new study. I added the fixed points on the bracket as well as the force that was applied. 

![myimage](A8.1begin.png)

| Design 1 | Coarse Mesh | Default Mesh | Fine Mesh |
| --- | --- | --- | ---|
| Max Stress (N/m^2 ) | 5.162e+06 | 5.811e+06 | 7.952+06 |
| Location | ![myimage](A8.1coarsevon.png) | ![myimage](A8.1defaultvon.png) | ![myimage](A8.1finevon.png) |
| Difference % |  | 12.57 | 36.84 |
| Max Deflection (mm) | 2.419e-03  | 2.007e-03 | 2.013e-03 |
| Location | ![myimage](A8.1coarsedef.png) | ![myimage](A8.1defaultdef.png) | ![myimage](A8.1findef.png) |
| Difference % | | 17.03 | 0.299 |
| Min SF | 48 | 43 | 31 |
| Location | ![myimage](A8.1coarsesf.png) | ![myimage](A8.1defaultsf.png) | ![myimage](A8.1finesf.png) |
| Difference % | | 10.42 | 27.91 |
| Mass | 0.671 lb | 0.671 lb | 0.671 lb |
| Number of elements | 1608 | 9364 | 63262 |

The component's results do not converge, I will use the finest mesh simulation's result to proceed with this assignment.

### Second Iteration

I added fillets to the non essential edges.

![myimage](A8.2.png)

| Design 2 | Coarse Mesh | Default Mesh | Fine Mesh |
| --- | --- | --- | ---|
| Max Stress (N/m^2 ) | 3.647e+06 | 3.601e+06 | 3.532e+06 |
| Location | ![myimage](A8.2coarsevon.png) | ![myimage](A8.2defaultvon.png) | ![myimage](A8.2finevon.png) |
| Difference % |  | 1.26 | 1.92 |
| Max Deflection (mm) | 8.216e-04  | 5.141e-04 | 5.081e-04 |
| Location | ![myimage](A8.2coarsedef.png) | ![myimage](A8.2defaultdef.png) | ![myimage](A8.2findef.png) |
| Difference % | | 37.43 | 1.17 |
| Min SF | 69 | 69 | 71 |
| Location | ![myimage](A8.2coarsesf.png) | ![myimage](A8.2defaultsf.png) | ![myimage](A8.2findsf.png) |
| Difference % | | 0 | 2.89 |
| Mass | 0.659 lb | 0.659 lb | 0.659 lb |
| Number of elements | 6678 | 13602 | 63529 |

The results from the default mesh and fine mesh converged at all three analysis points at less than 7% difference. I will proceed with the fine mesh results.

### Third Iteration

I shelled the big middle section to reduce weight. 

![myimage](A8.3.png)

| Design 3 | Coarse Mesh | Default Mesh | Fine Mesh |
| --- | --- | --- | ---|
| Max Stress (N/m^2 ) | 8.136e+06 | 8.360e+06 | 7.608e+06 |
| Location | ![myimage](A8.3coarsevon.png) | ![myimage](A8.3defaultvon.png) | ![myimage](A8.3finevon.png) |
| Difference % |  | 2.75 | 8.99 |
| Max Deflection (mm) | 2.059e-03  | 2.061e-03 | 2.084e-03 |
| Location | ![myimage](A8.3coarsedef.png) | ![myimage](A8.3defaultdef.png) | ![myimage](A8.3finedef.png) |
| Difference % | | 0.09 | 1.12 |
| Min SF | 31 | 30 | 33 |
| Location | ![myimage](A8.3coarsesf.png) | ![myimage](A8.3defaultsf.png) | ![myimage](A8.3finesf.png) |
| Difference % | | 3.22 | 10 |
| Mass | 0.386 lb | 0.386 lb | 0.386 lb |
| Number of elements | 6800 | 12829 | 68854 |

The results do not converge within 7% for mesh 2 and mesh 3. 

## Link

### First iteration

TO begin I started a new study on the link design from the previous assignment. I added the force and fixed geometry.

![myimage](A8Linkstudy.png)

| Design 1 | Coarse Mesh | Default Mesh | Fine Mesh |
| --- | --- | --- | ---|
| Max Stress (N/m^2 ) | 3.572e+08 | 3.620e+08 | 3.639e+08 |
| Location | ![myimage](link1coarsevon.png) | ![myimage](link1defaultvon.png) | ![myimage](link1finevon.png) |
| Difference % |  | 1.34 | 0.52 |
| Max Deflection (mm) | 4.125e-02  | 4.130e-02 | 4.130e-02 |
| Location | ![myimage](link1coarsedef.png) | ![myimage](link1defaultdef.png) | ![myimage](link1finedef.png) |
| Difference % | | 0.12 | 0 |
| Min SF | 0.69 | 0.69 | 0.69 |
| Location | ![myimage](link1coarsesf.png) | ![myimage](link1defaultsf.png) | ![myimage](link1finesf.png) |
| Difference % | | 0 | 0 |
| Mass | 0.041 lb | 0.041 lb | 0.041 lb |
| Number of elements | 2216 | 8717 | 39150 |

The results converged at below the 7% threshold, the fine mesh results were not needed but done for fun. 


### Second iteration

For the second iteration of the link I increased the width from 0.027 in to 0.100 in to try and increase the safety factor. 

![myimage](link2.png)

| Design 2 | Coarse Mesh | Default Mesh | Fine Mesh |
| --- | --- | --- | ---|
| Max Stress (N/m^2 ) | 9.693e+07 | 9.887e+08 | 9.925e+08 |
| Location | ![myimage](link1coarsevon.png) | ![myimage](link1defaultvon.png) | ![myimage](link1finevon.png) |
| Difference % |  | 2.00 | 0.38 |
| Max Deflection (mm) | 1.124e-02  | 1.126e-02 | 1.126e-02 |
| Location | ![myimage](link1coarsedef.png) | ![myimage](link1defaultdef.png) | ![myimage](link1finedef.png) |
| Difference % | | 0.18 | 0 |
| Min SF | 2.6 | 2.5 | 2.5 |
| Location | ![myimage](link1coarsesf.png) | ![myimage](link1defaultsf.png) | ![myimage](link1finesf.png) |
| Difference % | | 0 | 0 |
| Mass | 0.149 lb | 0.149 lb | 0.149 lb |
| Number of elements | 1502 | 11562 | 72357 |

The results converged at below the 7% threshold, the fine mesh results were not needed but done for fun. 













## Decide


## Communicate

I learned how different mesh sizes changes the approximation of the results. It is tempting to use fine mesh for every task but for more complicated analysis fine meshes may not be practical so we looked for convergence to ensure we did not waste time. We used these analysis to make changes so that our designs could be more lightweight, stronger, stiffer, or safer. 





### solidworks download

[Bracket](https://1drv.ms/u/c/3f1fcb01952d5efb/IQDTLF5dsNoiQp5yY80qsCDBAZEyf0kPrC31BWFqRWMAcGw?e=ZTXF5W)

[Bracket iteration#2](https://1drv.ms/u/c/3f1fcb01952d5efb/IQCGAhwBe6vcRp2EaUN6DWzoAZqBvPczPCr53evi06tKqIU?e=uJ7ubZ)

[Bracket iteration#3](https://1drv.ms/u/c/3f1fcb01952d5efb/IQBfnkKdG5T1QJr8fm9awKfoAR4mhdKra7AwX__XBSCPybo?e=sNiCMh)

[link](https://1drv.ms/u/c/3f1fcb01952d5efb/IQBVRse-T3-9R7sGSsghsh4EAefOseN2hoOvw_J5drr8nB0?e=wQOesq_)

[link iteration#2](https://1drv.ms/u/c/3f1fcb01952d5efb/IQBgsadDA5epTLZXJiYx1t3tAV4yUrGacBX70sC192u0DDA?e=MAL0Af)

