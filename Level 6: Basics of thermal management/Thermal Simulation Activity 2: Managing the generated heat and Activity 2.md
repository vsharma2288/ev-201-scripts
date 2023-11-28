**Let's get started by logging into your Simscale account.**

1. We will now initiate another thermal simulation to analyze the thermal behavior of IC 2n5298 with a heat sink. The heat sink we'll be using is the one provided in the kit. The choice of the heat sink for this simulation was made based on its availability in the market and its successful use in earlier BMS (Battery Management System) activities. Also we needed to compare the simulation result with measurement result later.  In this simulation, we aim to predict the temperature of the IC 2n5298 with the presence of the heat sink. This approach serves as one of the methods to effectively manage the heat generated in electronic components. Various open-source calculation tools are available to assist in the selection of the appropriate heat sink for specific electronics and heat dissipation requirements. 

**2. Go to "Dashboard" and Click "New Project"**

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2023-08-07/a82ce218-2e95-453b-a266-fce83f4e0a10/File.jpeg?tl_px=506,0&br_px=1366,480&force_format=png&width=560.0&wat_scale=50&wat=1&wat_opacity=0.7&wat_gravity=northwest&wat_url=https://colony-recorder.s3.us-west-1.amazonaws.com/images/watermarks/FB923C_standard.png&wat_pad=476,32)

**3. Type "Thermal Simulation Activity 2"**

**4. Click the "Describe your project..." field. Type "Thermal simulation of IC 2n5298 with heat sink". Rest of the inputs keep inline with first simulation.**

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2023-08-07/142b22ea-8127-4aa7-a4fa-bacea5a92946/File.jpeg?tl_px=272,0&br_px=1132,480&force_format=png&width=560.0&wat_scale=50&wat=1&wat_opacity=0.7&wat_gravity=northwest&wat_url=https://colony-recorder.s3.us-west-1.amazonaws.com/images/watermarks/FB923C_standard.png&wat_pad=262,134)

**5. Click "Create project"**

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2023-08-07/9d07c29a-8337-4ee0-90bb-12067ebc2811/File.jpeg?tl_px=396,176&br_px=1256,657&force_format=png&width=560.0&wat_scale=50&wat=1&wat_opacity=0.7&wat_gravity=northwest&wat_url=https://colony-recorder.s3.us-west-1.amazonaws.com/images/watermarks/FB923C_standard.png&wat_pad=262,179)

**6. To import the 3D CAD file, Click "from Onshape", login to Onshape account providing the credentials.**

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2023-08-07/dd0ce98d-ab08-447d-b9e8-334361d9aea7/File.jpeg?tl_px=163,51&br_px=1022,532&force_format=png&width=560.0&wat_scale=50&wat=1&wat_opacity=0.7&wat_gravity=northwest&wat_url=https://colony-recorder.s3.us-west-1.amazonaws.com/images/watermarks/FB923C_standard.png&wat_pad=262,138)

**7. Enter your Onshape account credentials**

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2023-08-07/8b57bb61-ac1e-4339-a878-4a41ece9d9c1/File.jpeg?tl_px=0,0&br_px=859,480&force_format=png&width=560.0&wat_scale=50&wat=1&wat_opacity=0.7&wat_gravity=northwest&wat_url=https://colony-recorder.s3.us-west-1.amazonaws.com/images/watermarks/FB923C_standard.png&wat_pad=256,127)

**8. Click "Sign in"**

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2023-08-07/c33728d4-9d41-46b1-9962-c88b057a245a/File.jpeg?tl_px=0,44&br_px=859,525&force_format=png&width=560.0&wat_scale=50&wat=1&wat_opacity=0.7&wat_gravity=northwest&wat_url=https://colony-recorder.s3.us-west-1.amazonaws.com/images/watermarks/FB923C_standard.png&wat_pad=188,138)

**9. Click "Authorize application"**

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2023-08-07/85a0f894-31f6-4791-8540-1f13b55fd9e9/File.jpeg?tl_px=0,138&br_px=859,619&force_format=png&width=560.0&wat_scale=50&wat=1&wat_opacity=0.7&wat_gravity=northwest&wat_url=https://colony-recorder.s3.us-west-1.amazonaws.com/images/watermarks/FB923C_standard.png&wat_pad=235,259)

**10. Click "Thermal activity CAD Data", which is the file you created in Onshape.**

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2023-08-07/2dfc03db-e671-4f65-b442-b3d9bd0ff461/File.jpeg?tl_px=0,0&br_px=859,480&force_format=png&width=560.0&wat_scale=50&wat=1&wat_opacity=0.7&wat_gravity=northwest&wat_url=https://colony-recorder.s3.us-west-1.amazonaws.com/images/watermarks/FB923C_standard.png&wat_pad=46,71)

**11. Select "Assembly of 2n5298 with heatsink" from the options. On the right side of the window, you will find the 3D view of the IC 2n5298 with the heatsink. Please double-check that you have chosen the correct 3D file. Once confirmed, click on "Import."

After completing this step, proceed to follow all the instructions outlined in the "Thermal simulation activity:01," continuing until the end of the "CAD import and CAD preparation for simulation" section.**

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2023-08-07/181229fe-556f-43cf-88f2-01f748461a42/File.jpeg?tl_px=39,138&br_px=899,619&force_format=png&width=560.0&wat_scale=50&wat=1&wat_opacity=0.7&wat_gravity=northwest&wat_url=https://colony-recorder.s3.us-west-1.amazonaws.com/images/watermarks/FB923C_standard.png&wat_pad=512,254)

**12. Now, let's begin defining the material and boundary conditions. We'll start by specifying the material for the external heat sink, which is made of aluminum. Click on "Solids" and choose "Aluminum" from the list of available materials. Keep the aluminum properties as default value.**

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2023-08-07/aaeebc19-b0fc-4880-9b01-dd2f11abc99e/File.jpeg?tl_px=19,0&br_px=879,480&force_format=png&width=560.0&wat_scale=50&wat=1&wat_opacity=0.7&wat_gravity=northwest&wat_url=https://colony-recorder.s3.us-west-1.amazonaws.com/images/watermarks/FB923C_standard.png&wat_pad=262,101)

**13. Click "Apply"**

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2023-08-07/5b363bfd-4371-464f-883c-eec585349fae/File.jpeg?tl_px=14,176&br_px=873,657&force_format=png&width=560.0&wat_scale=50&wat=1&wat_opacity=0.7&wat_gravity=northwest&wat_url=https://colony-recorder.s3.us-west-1.amazonaws.com/images/watermarks/FB923C_standard.png&wat_pad=262,234)

**14. Hide the flow volume**

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2023-08-07/047b1d1f-158c-456a-83d9-2d2668e23e31/File.jpeg?tl_px=506,60&br_px=1366,541&force_format=png&width=560.0&wat_scale=50&wat=1&wat_opacity=0.7&wat_gravity=northwest&wat_url=https://colony-recorder.s3.us-west-1.amazonaws.com/images/watermarks/FB923C_standard.png&wat_pad=526,138)

**15. Select the external heat sink**

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2023-08-07/411739d1-df06-4015-afcf-1ff20c829daf/File.jpeg?tl_px=363,101&br_px=1223,582&force_format=png&width=560.0&wat_scale=50&wat=1&wat_opacity=0.7&wat_gravity=northwest&wat_url=https://colony-recorder.s3.us-west-1.amazonaws.com/images/watermarks/FB923C_standard.png&wat_pad=262,138)

**16. Click here.**

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2023-08-07/7217cf6e-6bde-4385-9081-2c22bf2953a7/File.jpeg?tl_px=123,0&br_px=982,480&force_format=png&width=560.0&wat_scale=50&wat=1&wat_opacity=0.7&wat_gravity=northwest&wat_url=https://colony-recorder.s3.us-west-1.amazonaws.com/images/watermarks/FB923C_standard.png&wat_pad=262,30)

**17. From this point onwards, follow the instructions provided in "Thermal simulation activity:01" for the entire section on "Defining the material and boundary conditions" until the end.**

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2023-08-07/a2ad6915-2c33-48ab-ab41-3a2889ba960e/File.jpeg?tl_px=0,175&br_px=859,656&force_format=png&width=560.0&wat_scale=50&wat=1&wat_opacity=0.7&wat_gravity=northwest&wat_url=https://colony-recorder.s3.us-west-1.amazonaws.com/images/watermarks/FB923C_standard.png&wat_pad=133,138)

#### Replicate the steps outlined in the "Simulation pre-processing and starting of simulation Run" section from "Thermal simulation activity:01" exactly as they are for the pre-processing and initiation of the simulation run here.

**18. Type " Run 1_thermal activity 2" for the simulation run for identification.**

**19. Click "Start"**

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2023-08-07/a9f78e51-14fc-40f5-b645-29910bb7dcaf/File.jpeg?tl_px=46,41&br_px=905,522&force_format=png&width=560.0&wat_scale=50&wat=1&wat_opacity=0.7&wat_gravity=northwest&wat_url=https://colony-recorder.s3.us-west-1.amazonaws.com/images/watermarks/FB923C_standard.png&wat_pad=262,138)

**20. Run will take 40 to 60 mins of time. Let's wait for simulation run to complete.**

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2023-08-07/6bdf89dd-a7ad-4a60-9131-a481f00dcddf/File.jpeg?tl_px=7,0&br_px=867,480&force_format=png&width=560.0&wat_scale=50&wat=1&wat_opacity=0.7&wat_gravity=northwest&wat_url=https://colony-recorder.s3.us-west-1.amazonaws.com/images/watermarks/FB923C_standard.png&wat_pad=262,123)

**21. Wait till you get "Finished" message. Now simulation run is completed. It took 40mins to complete the run.**

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2023-08-07/52c9a043-3d09-4c6a-b501-d24edb709695/File.jpeg?tl_px=0,0&br_px=859,480&force_format=png&width=560.0&wat_scale=50&wat=1&wat_opacity=0.7&wat_gravity=northwest&wat_url=https://colony-recorder.s3.us-west-1.amazonaws.com/images/watermarks/FB923C_standard.png&wat_pad=218,52)

