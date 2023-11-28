https://vimeo.com/612931386


## Basic Introduction: Example 1

This will take you through a step-by-step process to analyze a block of iron sitting in a
magnetic field. The following sections will develop some additional concepts. 

### **1. Create model**

Select "nodes" from the toolbar (this is the farthest button on the left, with a small black
box:) and place 4 nodes for the corner of a box (at, for example, (0,0), (0,1.5), (1.5,0)
and (1.5,1.5)). Then, create 4 nodes for the corners of a smaller box inside the large box
(at, for instance, (0.5,0.5), (1,1), (0.5,1) and (1,0.5)). 

One can place nodes either by
moving the mouse pointer to the desired location and pressing the left mouse button, or
by pressing the TAB key and manually entering the point coordinates via a pop-up dialog.

Select "lines" from the toolbar (second button from the left with a blue line). To
select a node to be the endpoint of a line, click near the desired endpoint with the left
mouse button. By selecting the nodes for the larger box in sequence, one obtains lines between each of the nodes and result in a large connected box surrounding the 4 internal
nodes. Repeat the process for the internal nodes to create a small box inside a large box.

### **2. Add materials to the model**

Select "Properties|Materials Library" on the main menu. In the "Materials in Library" drop box that appears, select "Air" then click on "Add selected material to model".
Repeat for "M-19 Steel"

Click on "OK".
Define materials for each region.

https://do7js0tdxrds1.cloudfront.net/atjmzyer9r8s42pc7ftqok9r8ztv?response-content-disposition=inline%3B+filename%3D%22materials+library.jpg%22%3B&response-content-type=image%2Fjpeg&Expires=1701081822&Signature=el~I6wUwDq66jIzzbv01d0Gtoycx8gSArTI4mcScpZxMWctHptvT8CnXsiIhHAp7agtOPxix59XJftzLQO500pfqomYhMA~p~V7Oz3urNbr44VZDr11ovV971cvPKN1ynfuAjm39rEqPJ0TgBw2jym46rd~5wvzpFdj48K0pfUkGdpcI~pWjQqJxOC~ObY258PtzPsADqIspT73~k-wpsU-Tz3Sne1P0~w7nx7jThjA1rHCth7BSymiRxU2WQfOc0fdEVi4RoT6YJ3bO1XgOEUrCKOmRC6MeRqfeyAwc--1oTBlaZvv6i2mhdskU63z3zRida9iv9oY~jOHA6pS7~A__&Key-Pair-Id=K2Q3HDJ6ZAQGFF


Now click on "Block Labels" (the tool bar button with green circles), and place a
block label in the inner box and one in the outer box. Like node points, block labels can
be placed either by a click on the left mouse button, or via the <TAB> dialog.

>NOTE: If snap-to-grid is enabled then it may be difficult to place the block label in the
empty space. If this is the case, disable snap-to-grid by de-selecting the tool bar button
with the point and arrow.

Right click on the block label node for the outer box so that the node turns red, denoting
that it is selected. Press space to "open" the selected block label. 

A dialog will pop up
containing the properties assigned to the selected label. Set the "Block type" to "Air".
Uncheck the "Let Triangle choose Mesh Size" checkbox and enter "0.1" for the "Mesh
size". The mesh size parameter defines a constraint on the largest possible elements size
allowed in the associated section. The mesher attempts to fill the region with nearly
equilateral triangles in which the sides are approximately the same length as the specified
"Mesh size" parameter. When the "Let Triangle choose Mesh Size" box is checked, the
mesher is free to pick its own element size, usually resulting in a somewhat coarse mesh.
Repeat the same for the inner block label node and set the "Block type" to "M-19 Steel".

https://do7js0tdxrds1.cloudfront.net/psgb8px3dwp42349hg1exos2pghf?response-content-disposition=inline%3B+filename%3D%22adding+material.jpg%22%3B&response-content-type=image%2Fjpeg&Expires=1701081822&Signature=c78zH8sMdqpQXQmbkbLeqEjHadFSD9w2REMIOR0MC7QwkYK70TAWb13XECHu0Ae6plXtziZkF2DJz29UkJy2KA6E0GZIs0Ng4Y~loLUI9xaEJSaqj52mBYOHMaFlNKxWpr3iJzkNs3Rd~~Y1SjeZpnxK0COEOIcJiHWnUM2P6TgTt46~37fAJLRMhtv6haYCijgHEYvWl~3h3XrRtYQVK2kVvubTbs6I-zlIIDTlv~SRlk85sAjCjBQk7-s1AR3Hns4jF873fqSehtd~1mZUegdXSjN2ZL5OocnU~UPkuDtG4tUiNyqvxahqt-KK6KEDLUnEJSl8mFwp9BI4JoUu2Q__&Key-Pair-Id=K2Q3HDJ6ZAQGFF

#### 3. Create Boundary Conditions

Select "Properties|Boundary" from the menu bar, then click on the "Add Property"
button. Replace the name "New Boundary" with "Magnetic Field Source", and enter "1"
(one) for the A_0 parameter. Make sure the other fields are all zero, and the BC Type
(Boundary Condition type) is set to "Prescribed A". This means you have just defined a
boundary condition of 1 Wb/m, but you have yet to assign this condition to a particular
part of the model.

Repeat the above process but instead name the new boundary condition "Zero" which is a
zero magnetic flux plane, and set A_0 to "0" (zero).

Select "lines" from the toolbar then right-click on the left side of the large box. When it
turns red you have selected it. Now press the space bar and the "Segment Properties" window
will appear. From the top dropbox change the segment type from ":None:" to
"Magnetic Field Source". Repeat this process for the Left side of the inner box, but set
the segment type to "Zero".

https://do7js0tdxrds1.cloudfront.net/7zc9s7iwt1z7qol3k7adbk8vbmtf?response-content-disposition=inline%3B+filename%3D%22boundry+property.jpg%22%3B&response-content-type=image%2Fjpeg&Expires=1701081822&Signature=Ir8-iAmUdUkz6GdlMPHXXG9KNFiVUThuxkpi2wXxO5FY53UsJCUCMrsOl2Nm5HDVMgFfltHf2~uVmMTfmzCTbFsSr8xh32IjESeGuwE8ktJZt5V2gy09czdp3j8lY5fpHZkpQ6gabmtmxRoKGy5s2yLoiV~bqjNq2bFC6BQ~JfD~6fbuN5rzRFlLb3GQ53Vq1T7sRiqmbrlCzycIZ0hvm4cG8iCz-g9DjXD5n0HrhzjuOR3Om~wH8pyZRutbPYNUCjlArIMXTF7Aks0z2wuow0FD91h0Z4AO1lzNPIIm9OWTYFeZhQODNXtGZPWI8-gdESMBfGRGbNR18tofaUWPoQ__&Key-Pair-Id=K2Q3HDJ6ZAQGFF

Select "Problem" from the menu bar and make sure the frequency is set to zero, the
problem type is planar, and the length unit is set to meters.

https://do7js0tdxrds1.cloudfront.net/hl8158ltleyh4qbvnfqftk3fksnn?response-content-disposition=inline%3B+filename%3D%22problem+definition.jpg%22%3B&response-content-type=image%2Fjpeg&Expires=1701081822&Signature=rdJEhLIBjpWA9k23992TZXkZ-hOIuA0bCCOj-6TJnDTdzXBxTTr~658YqF4HaI56TmokyR0CQHZYv6g6vafCy8~szgLZ83y8Agkoe~IHx55z0N4V825RiYAK-YvLB4F4itscsWwUE3zv78f~USNVv~SToEnyMvS8wKYmvhoLt7Oo5B06qN6KKmxxQGNuuHU8hrApES00vi4XW9UYrkmQ4AuZrsWOzV7bFBtbwETuk6D0nTyTt75q4elR7w94nyGXkNePUdyV-UPq4ga8k3cXGjSHbhCCgOpBzLAnFojeGVf6H~sbhr9Umv34jiPCMPMG~4guZ-a6StnFzZgOAtXA3Q__&Key-Pair-Id=K2Q3HDJ6ZAQGFF

#### 4. Generate Mesh and Run FEA

Now save the file and click on the toolbar button with yellow mesh, This action
generates a triangular mesh for your problem. If the mesh spacing seems too fine or too
coarse you can select block labels or line segments and adjust the mesh size defined in
the properties of each object. 

Once the mesh has been generated, click on the "turn the
crank" button to run the FEA algorithm over your model.

Processing status information will be displayed. 

>If the progress bars do not seem to be
moving then you should probably cancel the calculation. This can occur if insufficient
boundary conditions have been specified. 

For this particular problem, the calculations
should be completed within a few seconds. 

There is no confirmation for when the
calculations are complete, the status window just disappears when the processing is
finished.


### 5. Display Results
Click on the glasses icon to start FEMM View. 

In FEMM View, you can click on the
purple shaded button to generate a colour field intensity plot. When the dialogue box comes
up, select the "Show flux density" box, and accept the other default values. Click on
"OK".

https://do7js0tdxrds1.cloudfront.net/fdkphdm0kfgi2ovi58vsdytd7ena?response-content-disposition=inline%3B+filename%3D%22result.jpg%22%3B&response-content-type=image%2Fjpeg&Expires=1701081822&Signature=c7w~bJuheVrF9YMDqYucuJX8unE92eexaYjk~eQ~vx1fnwlxCK0qN51sDeL8j1nS3sLTqoORIHkO7QdDUfeMzyUJeNcQNt~atiYl3F2Suw0EowMJkqKM0ujzGF-6otdIt2~h8nWF77VSPLKj8HidMIqXdMblrmbGVJw1Znk-bzdRzaOFbprp6-JM0nQbeKkAxqOXoC86Iw34F0eFBroZeWpDFe83BlTaZU~a7k8hZCcepWPQPCMAE6FeOJuSOxHzb9M-U0e35-aW~QqZXd7gfszOts6MBmHjvROqe~73GV2X0rrm53jZ1etUCYE9AsjMXtg3NX~G3Pc4emXo7sh0qw__&Key-Pair-Id=K2Q3HDJ6ZAQGFF

### From this basic introduction you should have gained the following principles:
     •  How to create your model space using nodes and lines.
     •  How to add material types to your model and how to assign them to regions.
     •  How to specify the finite element mesh size.
     •  How to define a boundary for your model.
     •  How to define and apply boundary conditions.
     •  How to calculate and plot your results.