# A2 – Truss Stress Analysis

## Objective
The objective for this assignment is to design a truss, analyze the truss, determine pin sizes needed for the truss, and then model the truss in CAD software. 

## Analyze

### Design

![myimage](trussss.png)

To start we were given that point A is a pin and point B is a roller. The distances given for a is 0.4 m and for distance b it is 0.3 m. We were told to pick a value for P, I chose 25 KN. The planar truss will be designed using AISI 1020 Steel.

### Sketch and internal forces
![myimage](sketch.jpeg)

This is the sketch of my truss. It follows the given measurements and labels the joints. It has the load P at joint C and D. My next steps will be to symbolically and numerically solve the internal forces of the truss.

![myimage](trusssym.png) ![myimage](trussnum.png)

Initially I found the support reactions of the truss. I then symbolically solved joint B, E, C, D, and lastly F. Once I found all of the members forces symbolically I solved the members numerically using P=25 kn. I listed all the forces on the second image. Next I will calculate the required cross-sectional area.

### Cross-sectional area and weight

![myimage](weight-1.png)

I listed the knowns and unknowns. I used the largest force and I found the yield strength of AISI 1020 in Solidworks which was 357.57 MPa, I found the required cross sectional area. I found the formula for rectangular hollow tube. The density of AISI 1020 in solidworks was ρ=7870 Kg/m^3. I decided to use a wall thickness of 3 mm, an outside width of 28 mm, and an outside height of 25 mm. I found the mass of 8.21 kg and weight of 80.54 N

### Pin Calculations

![myimage](pincalculations..png)

The material and properties of the pin were given. I used the largest force of 27.78 KN. I converted the force to lbf, and used the equation Amin= FN/Ty, F being the force, N being the safety factor, and Ty is shear yield strength. This gave me the minimum cross-section area of 94.8 mm^2. I used the area to find the minimum diameter of 10.98mm which I rounded up to 11mm. I chose a length of 30mm to ensure the pins would have space for a locking mechanism. I calculated the weight of the pins to be 0.2153 N.

### Solidworks model

![myimage](truss.sketch.png)
![myimage](truss.finished.png)
![myimage](pina2.png.png)

To begin I created a solid outline and extruded it from the midpoint. I then sketched triangles to eliminate the material from the truss and leave just the supports. I created pin holes for the connection pins. I modeled the pins as cylinders with a diameter of 11mm and a length of 30 mm. 

![myimage](truss.mass.png)
![myimage](pin.mass.png)

The estimated mass of the truss was 8.21 kg and the estimated mass of one pin was 0.02195 kg. The mass according to solidworks for the truss was 17.69 kg and for the pin it was 0.02 kg. The pins were very close in mass since they are a simple shape to calculate mass. The calculations for the truss's mass modeled it as hollow with a wall thickness of 3 mm, in solidworks it is not modeled as hollow so that is why there is a discrepancy.


## Decide

I chose to add support members to the truss and not use just the initial trapezoidal shape. It allows the members to transfer loads. I decided for member the diagonal member to go from point C to the point E to try and transfer the upward force of P more evenly among the truss. 

## Communicate

I learned how to design a trust and take into account the yield strength of the materials. I also learned how to design with a safety factor in mind to prevent buckling and yield failures. 

It took me approximately 10 hours to complete my work. 
