You will now create a model of a current-carrying coil wire in an axisymmetric system with a better boundary condition. Imagine a 5 cm radius cylinder with a 1 cm copper wire wound around it. We are going to model the field produced by this single turn of the coil using a better approximation of an infinite boundary condition (i.e. ideally, the field goesto zero at infinity, not at some relatively near artificial boundary).

>This exercise will prepare you to design a 2 pole motor for the next assignment. Right now you are simulating a motor pole.


https://do7js0tdxrds1.cloudfront.net/0jutn5jcmcdp0e5svmdmytj44bo7?response-content-disposition=inline%3B+filename%3D%22example+2.jpg%22%3B&response-content-type=image%2Fjpeg&Expires=1701082009&Signature=g8wQ-voMMUbKHbwwpFSzUFMHtIgPYBXrXAalr-oIGVUsMnQ-VL~x8wkpYBu5L9tgDucX8eIebSZTp2TG6eXuW1J8HRn0rImUR4TvQ5Rj0K5L-6XQtIdt9217JBAU7L0QfJwWjhwBK3~0jr96vkVCiW4jEroUSh7VqcFsDW6wZD6ZUDkzGJkS5NKS8yye1e5bCW2lK1FRNBIP03xHVLKCr867zWtg5~umlCl30jQZLZVCa9aKKpw8Ybs87phQGvWZjjjKpwTmgs0XloHYJREY~9pScAAqAkTjGNouwjbzD6N7uh1ZSAXLPppRkRmnTZLHahggs3uG7hIQiOzb3Y04CA__&Key-Pair-Id=K2Q3HDJ6ZAQGFF

1. First set the "Problem" properties to 0 Hz, axisymmetric, and units of centimeters. In this case, the vertical axis is the radial axis of the problem (or imagine it as a line of symmetry). 

2. Change the "Grid Size" to 1, meaning each dot represents 1 cm, and select snap-to-grid by pushing in the toolbar icon. Snap-to-grid allows points and block labels to be placed exactly on grid points using clicks of the left mouse button.

3. Find the r = 0, z = 0 point (the system origin). This may require zooming out. Place a node at the origin.

4. Place nodes at (r, z) = (0,15), (0,-15), and (5,0), (6,0) (refer to the left side of the status bar at the bottom of the screen for a read-out of the current mouse pointer
position).

5. Connect lines between (0,0) and (0,15) and (0,-15). This is the axis of rotation for this
axisymmetric problem.

6. Select the arc toolbar button. Select the (0,-15) point (bottom point), then select
the (0,15) point (top point). When the dialog box comes up, enter "180" for "Arc
Angle". Arcs are drawn counterclockwise, so this will draw the right side arc
between the two points and the arc will cover 180 degrees (half a circle).

7. Now select the (5,0) point followed by the (6,0) point, and enter "180" for "Arc
Angle". Repeat in the opposite order to complete the top half of the circle.

8. Zoom in on the circle section by selecting "View" then "Window" and draw a box
around the circle.

9. Deselect "snap-to-grid" in the `Grid` menu and place a block label by selecting the `green circle logo` on the toolbar or by selecting the `Operations - > Node` option, place one node inside the circle, and one outside the circle.

10. Add "Air" and "Copper" to the model materials using the `Properties - > Materials
Library` dialog box from the menu bar (Select `solid-non magnetic conductors `then drag and drop `copper` into model materials).

11. Select "Properties" then "Materials" from the menu bar and modify Copper. Change
the "`J_re, MA/m^2`" box from "0" to "5", which corresponds to 5,000,000 amps per
square meter current density, or 5 A/mm2, or approximately 390 A along a 1 cm
diameter wire.

12. Select the block label inside the circle by right-clicking with the mouse near the green
node. Change the "Block type" to Copper, and the "Mesh size" to 0.1 (since 0.1 of
1 cm (remember base units are cm) equals 1 mm, this is mesh size). Do the same for
the outer block label node but assign it to "Air" and "Mesh size" to 1 (0.1 is too fine a
scale for such a large region).

13. Click on the blank page toolbar button. This button causes the view to zoom out
so that the whole page is visible.

14. Select "Properties | Boundary" and then "Add Property". Rename your new boundary
"Infinite Estimate" and change the "BC Type" to "Mixed". Given that the system
under analysis is close to the center of an arc (usually either a full or half circle), "`c0`
coefficient" can be set to `1/(4 p r * 10-7)` where `r` is the radius of the arc in meters. In
this case, `r = 0.15 m`, so `c0 = 5305165`. All the other values should be zero (including
`c1` coefficient).

https://vimeo.com/623438620


15. Select the half-circle by right-clicking on or near it (the "Arc" toolbar button must also
be depressed). Press space and assign "Infinite Estimate" to "Boundary cond.".
16. Now perform the calculation and activate FEMMView to display the magnetic field
produced by the current in the wire. 


>Note that the vertical side of the semi-circle boundary (along the radial axis) does not
have any boundary condition assigned--a zero potential boundary condition is defined to
the axis of rotation in axisymmetric problems by default. 

>Also note how the magnetic
field lines radiate through the outer arc boundary as if heading to infinity. This is due to
the use of an impedance boundary condition on the outer boundary, which closely mimics
the behaviour of the coil in unbounded free space. 

```
More information on so-called "open"
boundary conditions are available in the FEMM User Manual appendices. 
```

For comparison
purposes, define a boundary condition with "Prescribed A" and set the A_x coefficients
to zero. Name this "Zero" and change the arc properties from "Infinite Estimate" to
"Zero" and compare the results. With a "Zero" outer boundary, no field crosses the outer
boundary.

 *FEMM User Manual*