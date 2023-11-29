### Step 1: Start a new Magnetics problem.

From the menu bar select 'problem' and check that you are using the correct units with respect to your DXF file and that have set up a planar simulation. You will also want to check that the 'depth' of your simulation matches the length of your rotor. In this case, our rotor was 13 mm long.

https://do7js0tdxrds1.cloudfront.net/w3584puryx8qseu20vi66t3j32q1?response-content-disposition=inline%3B+filename%3D%22problem.jpg%22%3B&response-content-type=image%2Fjpeg&Expires=1701252941&Signature=XZB5zkAzZODa6WfEEA9q1RwIXX0myEzd~WOsOuOKCI9a7Wk47hvSY9BBvoP5YjZ4mqjAc7x2PeDSh-Bvk5htpnfVg3h5tYRmiZvwnD0Z46jOZTId~XGzrX7iKNBrKLOhAD3TRdv6KNfgF-o~ZCCTYkU0zWJhizUK8J0r7pHmgaS0eQAw8JJk-DPQM1ril3E9qgbCA5oFDpXjFAiCEq2lrZ1B9rhffty4CcYAAtG6EBp8CWmVjvGBpieSygVZyi~YEwDyF0~UAxaPBMLDkx3UzuOWQv4aaxt7YVGFJn-~9XSSR4bZYYrYVoXZWE8fGQuRoAm7-JXZInKcZj2zNtTVLA__&Key-Pair-Id=K2Q3HDJ6ZAQGFF

### Step 2: Import DXF

The next step is to import your DXF file(s) using the file → import DXF option. 

>Note that it is also important that the centre of your model be located at point (0,0) for torque estimation to be conducted later.


### Step 2: Import DXF

The next step is to import your DXF file(s) using the file → import DXF option. 

>Note that it is also important that the centre of your model be located at point (0,0) for torque estimation to be conducted later.


### Step 4: Define the winding type

The windings were then assigned based on the number of turns and the number of strands.

1. Create a new 'property' using the property definition dialogue box. 

2. Select/type `plain stranded wire with a 0.34 mm diameter and 4 strands` and then assign the same properties used by the other copper conductors.

https://do7js0tdxrds1.cloudfront.net/o5eoljbrsysailvs1r0kgz0zgu3f?response-content-disposition=inline%3B+filename%3D%22block+property+2.jpg%22%3B&response-content-type=image%2Fjpeg&Expires=1701252941&Signature=PQyaK~LavQZbU~ztCe8166CWmIEjE4Kl36CazSPUrKRIb3TnEaTLnQMxdvx1Zbb674tLtTCV1GHUlN-UuUAbloBw1ZS91AdB~Y3KY2I8OPHy3utdUZj1H~hYpwJtHZ-c3nXSf335qSQp62BZzF0CBjrPGQKMSDH3jLzEQHodkfYT8Z9m0J16SIZAsVb-U0jHecnx3iqWT74u~rWYzRa5xsYsvpCG1Mjz2UH6ZCtzybu7mpFzPqlleFBRpGDC-lOIjn1MNs9z4JfABrL8T9nWGSbQKfxvHJCgQrXPI41RwLb0W5YjhFx0j1KA3cpktxho7U3GEg9PmojHC0n24Ycvvw__&Key-Pair-Id=K2Q3HDJ6ZAQGFF

### Step 5: Determining the winding order

The Winding order of the motor was determined using this [winding layout tool](http://www.bavaria-direct.co.za/scheme/calculator/). 

By selecting `12 slots, 14 poles`, `two-layer winding` (single winding per tooth as opposed to a single winding for every second tooth) and selecting the type as `D` for Delta the following is seen.

https://do7js0tdxrds1.cloudfront.net/o0jkg50hl1ukafh66phbjt566hpm?response-content-disposition=inline%3B+filename%3D%22copper+winding+direction.jpg%22%3B&response-content-type=image%2Fjpeg&Expires=1701252941&Signature=G-Yz92~GgxNWvqs4-Hd17FD~nf6~ftZdXMT6QobnerlEUMsWkYBCFBWjQ2NDTZy3b29Um2PUrGtHQX5R3ssmiqsn8VhPmlHrSAyW3xYpH2Xqt-564knFjGBeKg2rtZsyyz7wnQUYP6fG~NTh9tA5qxDwpdHOlBDGZnLwW9UYs48MgWNXn9bLeE6Qdc0fwQt0Hh12qree7k4yuPuiergQ~GtK1zeCbYPFngq4tK5~jiYndKdau8qokNlSiDCzyB6xcpEux~QZgKbYStQ3XxHiPTO7mXJwDjWouYb00R0CAT7oQZediDRElrXTlO-4TA2lxDj0N6eZH1UIhlUCQZMMyw__&Key-Pair-Id=K2Q3HDJ6ZAQGFF

Using this as a template, the winding phase and direction (either into or out of the page) can be assigned.

### Step 6: Assigning Materials and windings

https://do7js0tdxrds1.cloudfront.net/vgwwoq56glkoc7j4tujypmyhwx13?response-content-disposition=inline%3B+filename%3D%22assigning+materials.jpg%22%3B&response-content-type=image%2Fjpeg&Expires=1701252941&Signature=VmodhmAys4L-1b1Ur3fe8KvJoOkTBVrRMn3U-opgN4E1uuFkb-3VH4yQi3kabVbJAAP57PWs32Xtar4LPDUEay8wbqq-WRrA3eFSVybSuc4F8Wr-rEWLmFYBnXnltzZBkfS6X6n1KvbQEtVp-hrj~Q1oTnIY7~fB3MebQuB17HTniAuj~gLse2ZgZ4kOxy-5X4kSBg8o9wL6sZOvzj6gHN9V3dZOkqnwDUPpaU3bCOg57VDKHsCx98MSmzmt3vCj-Nd9e3aUxuh0TmU3VjtSs3myq1ARnsEp6Ci2n1S3X9~zKP~xUhtJBTy5oNHyHXBunWjD8fWk-QF1buI1sz0HkA__&Key-Pair-Id=K2Q3HDJ6ZAQGFF
Caption: With all the materials properties assigned we see the above image.

>No need to worry, you will get an already filled DXF in order to save time.

* The regions filled by air were assigned (one for the air gap region inside the rotor bell and one for outside the motor).

* The open boundary builder (circle within a circle button) was used to set the boundary conditions and default settings in the boundary builder are fine here.

### Step 6: Estimating winding current

Since this motor is driven using field-oriented control (FOC) we need only supply a current to one phase and a current opposite in sign, and twice as small, for the other two phases as per the figure below.

https://do7js0tdxrds1.cloudfront.net/6jvwqg8xpvg6duv3p6b9go9bqbiv?response-content-disposition=inline%3B+filename%3D%22ezgif-2-dfe4333f7199.jpg%22%3B&response-content-type=image%2Fjpeg&Expires=1701252941&Signature=VMzmuw9CUgO9d640wlMKt~d2AyRixc8gvEiTzOIK1ElszRUzCB~o6Kieyos8hama53CYhdZaLJHsVQWZ7XJM-9HlquJDy5o18tqAydCcYKIrQKq8dppnJRGxAkoSyok8zj4B8xNY5vnocLQ4EXMFx0pusnWQxifcHFQyTocqfQ2PQ2SlLVkOJzlq5vKCC2yYboUMZVSd3rOLG~PuWHzQvFf4CcgO5QGYM8TUyyGj0ITjlq4DGSbb-tvYfgVGxJq~2L0cV78jP~RGDX5mcMKY4xoNt9uyQCPjw5oMxs~1OkFRtMCKltUUF46EEaSC6NAYuEhvaKvBnCBVnqr2t8AkGA__&Key-Pair-Id=K2Q3HDJ6ZAQGFF

https://do7js0tdxrds1.cloudfront.net/6jvwqg8xpvg6duv3p6b9go9bqbiv?response-content-disposition=inline%3B+filename%3D%22ezgif-2-dfe4333f7199.jpg%22%3B&response-content-type=image%2Fjpeg&Expires=1701252941&Signature=VMzmuw9CUgO9d640wlMKt~d2AyRixc8gvEiTzOIK1ElszRUzCB~o6Kieyos8hama53CYhdZaLJHsVQWZ7XJM-9HlquJDy5o18tqAydCcYKIrQKq8dppnJRGxAkoSyok8zj4B8xNY5vnocLQ4EXMFx0pusnWQxifcHFQyTocqfQ2PQ2SlLVkOJzlq5vKCC2yYboUMZVSd3rOLG~PuWHzQvFf4CcgO5QGYM8TUyyGj0ITjlq4DGSbb-tvYfgVGxJq~2L0cV78jP~RGDX5mcMKY4xoNt9uyQCPjw5oMxs~1OkFRtMCKltUUF46EEaSC6NAYuEhvaKvBnCBVnqr2t8AkGA__&Key-Pair-Id=K2Q3HDJ6ZAQGFF

*Download this already filled file to make things easier.*

https://vimeo.com/669990929