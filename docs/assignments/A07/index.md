# A7 – [FEA on Bracket]

## Objective

The objective for this assignment is to optimize the design of our bracket and link from the previous assignment #5. We will use finite element analysis to help assist us with modifications to improve our bracket. The FEA will give us data on the strength, stiffness, and safety factor of our bracket, using that date we will try to make it more lightweight. We are also tasked with documenting our processes and decision choices. 

## Analyze

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

| Design 1 | Coarse Mesh | Default Mesh | Fine Mesh |
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


## Decide


## Communicate

