Now that we have the simulation up and running, let's estimate the torque of your motor. 

The torque constant (K~t~) of an electric motor can be estimated easily using FEMM with just 1 step. 

> To get peak torque values, make sure the rotor is rotated, in our motor we will be rotating the motor by 90 electrical degrees.

`360 electrical degrees is equal to 360 mechanical degrees divided by the number of pole pairs, which in this case is 7`

Simulating the 12n14p motor with the rotor 90 electrical degrees looks like the following.

https://do7js0tdxrds1.cloudfront.net/asppu9j3kmcyouxzrp8fzdj0didj?response-content-disposition=inline%3B+filename%3D%22motor+output.jpg%22%3B&response-content-type=image%2Fjpeg&Expires=1701253513&Signature=dEgXZYgNc01yFFycA75LDYDWBHytC1pw9vmjRMWbeWb4zpfpom1P953ASdNFwIvNchey7ueeVhLMQ5V6Fu9Xr-~gRQpCVAEetgFPU6~uihT6Or~xCQjwrroZYSEA42HRnNAnEIIBENyazft6a0AyMf6uOOrHHRuRrYd6LqMWTOA9oyBzhUvhiCWovoMreQijlH~0iijw5TrQAh1QzmuztCd52xDxfM1RiE8RhQw9aqD2WSGykefI2EKe20AXevsuueoTl1bEe8drb~cVqNamo9TKR8o4CX8jlS9bB8-7A8z59Thh5to4hhOrhZCRz-IGPAc3JYWnY0m2ApbMGy4PjQ__&Key-Pair-Id=K2Q3HDJ6ZAQGFF


Next,

To determine the torque produced, the rotor needs to be selected using the area selection tool (green box inside four points) by clicking on each of the magnets and the rotor bell.

With the rotor selected, we can find the torque around point `0.0` using the integrate option and `'Torque via Weighted Stress Tensor'` selection from the drop-down menu, as recommended in the FEMM manual.

https://do7js0tdxrds1.cloudfront.net/yop02sfaq7g7rvp2e397pt5c44hb?response-content-disposition=inline%3B+filename%3D%22torque+by+weighted+stress+tensor.jpg%22%3B&response-content-type=image%2Fjpeg&Expires=1701253513&Signature=rrstiPXPr9JVFwQzgiiKNg37yPpuJcOnMY84iTghtdqABzuJAUcjSVceWB4020kr7-f3vBkEM9XvRFU9N2zingLJB~Wh6~3Duxta6DCSAbJWGL~z8MMv45NiYBNHg0j8YplhXlXsQ7cERQK8hqk~OvFgK91ztuP-QD~YKwOFrE~rPM3uYXpetPCoEl9LXWnxZtC4TkBfLBD3DWI9Rs~C6aE4zYbHHIMx2AhKXjUFMFhG3SSDldPlLrxhEJLppEUYrXSUG9ROwrZlFpAaBIlhyOfZuxG-f57IM-UvqVM9J5GTiguPUbtLaCPCdNxRM2LbwFH7UN443Wq9O1W5ftZVLg__&Key-Pair-Id=K2Q3HDJ6ZAQGFF

Now that we have the torque figure, let's move on to estimate Back EMF and K~v~.