#### Defining the material and boundary conditions

**39. An essential step in any finite element simulation is accurately assigning materials and capturing appropriate boundary conditions. Let's begin by assigning materials now, starting with the Flow region. Since we know IC2n5298 in the BMS board is surrounded by air, we will assign this material to the flow region. Next, click on "Fluids" under "Materials" to proceed.**

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2023-08-09/ad2eb284-464c-4e57-bdcc-68e98e399a40/File.jpeg?tl_px=0,133&br_px=859,614&force_format=png&width=560.0&wat_scale=50&wat=1&wat_opacity=0.7&wat_gravity=northwest&wat_url=https://colony-recorder.s3.us-west-1.amazonaws.com/images/watermarks/FB923C_standard.png&wat_pad=63,138)

**40. Click on "Air"**

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2023-08-09/61ff0757-b2e7-4d32-a03c-014035b52ec3/File.jpeg?

**42. Click "No Volumes assigned"**

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2023-08-09/1bffe1a0-53a5-4fa3-b3ef-b000d85ea708/File.jpeg?tl_px=22,176&br_px=882,657&force_format=png&width=560.0&wat_scale=50&wat=1&wat_opacity=0.7&wat_gravity=northwest&wat_url=https://colony-recorder.s3.us-west-1.amazonaws.com/images/watermarks/FB923C_standard.png&wat_pad=262,186)

**43. Click "Flow region" as shown, ensure the "Flow region" is selected now.**

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2023-08-09/e8cbd39f-836b-499c-a0b7-0dc96fd5e2aa/File.jpeg?tl_px=506,34&br_px=1366,515&force_format=png&width=560.0&wat_scale=50&wat=1&wat_opacity=0.7&wat_gravity=northwest&wat_url=https://colony-recorder.s3.us-west-1.amazonaws.com/images/watermarks/FB923C_standard.png&wat_pad=461,138)

**44. Click here.**

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2023-08-09/9e4c6c79-b94a-4b30-a2f4-7739405d49e2/File.jpeg?tl_px=54,0&br_px=1037,549&force_format=png&width=560.0&wat_scale=50&wat=1&wat_opacity=0.7&wat_gravity=northwest&wat_url=https://colony-recorder.s3.us-west-1.amazonaws.com/images/watermarks/FB923C_standard.png&wat_pad=262,29)

**45. Now let's assign the material for IC 2n5298. Here are the material list.**      
1) Heat sink on IC: Aluminum                                                                                 
2) Legs of IC (all three) : Brass                                                                               
3) Plastic coating of IC: Epoxy                                                                               
 Let's assign these materials, click "Solids"

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2023-08-09/3af7fdfc-7e1d-4af2-9f3d-2e82bf03adee/File.jpeg?tl_px=0,176&br_px=859,657&force_format=png&width=560.0&wat_scale=50&wat=1&wat_opacity=0.7&wat_gravity=northwest&wat_url=https://colony-recorder.s3.us-west-1.amazonaws.com/images/watermarks/FB923C_standard.png&wat_pad=67,147)

**46. Select "Aluminium," and for the properties of aluminum, retain the default values without making any changes. These default values are suitable for the current simulation and do not require any modification.**

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2023-08-09/a282e621-5d94-4c4d-bc97-a1e688bd572b/File.jpeg?tl_px=0,0&br_px=859,480&force_format=png&width=560.0&wat_scale=50&wat=1&wat_opacity=0.7&wat_gravity=northwest&wat_url=https://colony-recorder.s3.us-west-1.amazonaws.com/images/watermarks/FB923C_standard.png&wat_pad=256,106)

**47. Click "Apply"**

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2023-08-09/f5d769b4-4742-4705-b03f-1060661384e1/File.jpeg?tl_px=0,176&br_px=859,657&force_format=png&width=560.0&wat_scale=50&wat=1&wat_opacity=0.7&wat_gravity=northwest&wat_url=https://colony-recorder.s3.us-west-1.amazonaws.com/images/watermarks/FB923C_standard.png&wat_pad=250,233)

**48. Hide the flow region, click on 'heat sink' of the IC.**

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2023-08-09/b510e5a8-2b55-4644-9016-3e9ced0cb3ab/File.jpeg?tl_px=242,18&br_px=1102,499&force_format=png&width=560.0&wat_scale=50&wat=1&wat_opacity=0.7&wat_gravity=northwest&wat_url=https://colony-recorder.s3.us-west-1.amazonaws.com/images/watermarks/FB923C_standard.png&wat_pad=262,138)

**49. Ensure heat sink is rightly selected and click here, confirm this with Assigned Volume (1) field as well. 1 indicates only 1 volume is selected, which is correct here.**

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2023-08-09/5418bf07-9714-4639-8224-273676851815/File.jpeg?tl_px=117,0&br_px=976,480&force_format=png&width=560.0&wat_scale=50&wat=1&wat_opacity=0.7&wat_gravity=northwest&wat_url=https://colony-recorder.s3.us-west-1.amazonaws.com/images/watermarks/FB923C_standard.png&wat_pad=262,35)

**50. Click "Solids" again and select Epoxy**

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2023-08-09/7c3d32e7-73f9-48da-8b5b-91447e582c52/File.jpeg?tl_px=0,176&br_px=859,657&force_format=png&width=560.0&wat_scale=50&wat=1&wat_opacity=0.7&wat_gravity=northwest&wat_url=https://colony-recorder.s3.us-west-1.amazonaws.com/images/watermarks/FB923C_standard.png&wat_pad=130,145)

**51. Click on "Epoxy," and as expected, the default values are sufficient for the simulation.**

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2023-08-09/5cf9d0a4-6da2-4bb8-872e-8779460c114a/File.jpeg?tl_px=0,140&br_px=859,621&force_format=png&width=560.0&wat_scale=50&wat=1&wat_opacity=0.7&wat_gravity=northwest&wat_url=https://colony-recorder.s3.us-west-1.amazonaws.com/images/watermarks/FB923C_standard.png&wat_pad=256,138)

**52. Click "Apply"**

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2023-08-09/d2e4240a-83ca-4cc8-b6a1-c58c49839993/File.jpeg?tl_px=8,176&br_px=867,657&force_format=png&width=560.0&wat_scale=50&wat=1&wat_opacity=0.7&wat_gravity=northwest&wat_url=https://colony-recorder.s3.us-west-1.amazonaws.com/images/watermarks/FB923C_standard.png&wat_pad=262,230)

**53. Select the IC plastic housing.**

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2023-08-09/572f6ba9-b448-44b6-bc6c-a1aa8bcf2f35/File.jpeg?tl_px=247,124&br_px=1107,605&force_format=png&width=560.0&wat_scale=50&wat=1&wat_opacity=0.7&wat_gravity=northwest&wat_url=https://colony-recorder.s3.us-west-1.amazonaws.com/images/watermarks/FB923C_standard.png&wat_pad=262,138)

**54. Click here, ensuring that right volume is picked, even here only 1 volume need to be picked.**

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2023-08-09/9a5e1b02-cf6d-47c9-8115-c32b888d51aa/File.jpeg?tl_px=122,0&br_px=981,480&force_format=png&width=560.0&wat_scale=50&wat=1&wat_opacity=0.7&wat_gravity=northwest&wat_url=https://colony-recorder.s3.us-west-1.amazonaws.com/images/watermarks/FB923C_standard.png&wat_pad=262,35)

**55. Again click on "Solids" and select "Brass"**

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2023-08-09/902fb29c-2956-4e0a-a3e5-58742772bbcb/File.jpeg?tl_px=0,176&br_px=859,657&force_format=png&width=560.0&wat_scale=50&wat=1&wat_opacity=0.7&wat_gravity=northwest&wat_url=https://colony-recorder.s3.us-west-1.amazonaws.com/images/watermarks/FB923C_standard.png&wat_pad=132,149)

**56. Click "Brass", and default values are ok here as well.**

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2023-08-09/8344503d-97f8-4e3f-abdd-806d6762f64e/File.jpeg?tl_px=4,0&br_px=863,480&force_format=png&width=560.0&wat_scale=50&wat=1&wat_opacity=0.7&wat_gravity=northwest&wat_url=https://colony-recorder.s3.us-west-1.amazonaws.com/images/watermarks/FB923C_standard.png&wat_pad=262,128)

**57. Click "Apply"**

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2023-08-09/498262ed-6d0d-4f52-8676-9f2b3eecee80/File.jpeg?tl_px=13,176&br_px=872,657&force_format=png&width=560.0&wat_scale=50&wat=1&wat_opacity=0.7&wat_gravity=northwest&wat_url=https://colony-recorder.s3.us-west-1.amazonaws.com/images/watermarks/FB923C_standard.png&wat_pad=262,230)

**58. Select all three legs of IC**

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2023-08-09/36c7f5d6-d5af-40c3-acd5-133445567c00/File.jpeg?tl_px=202,176&br_px=1062,657&force_format=png&width=560.0&wat_scale=50&wat=1&wat_opacity=0.7&wat_gravity=northwest&wat_url=https://colony-recorder.s3.us-west-1.amazonaws.com/images/watermarks/FB923C_standard.png&wat_pad=262,160)

**59. Click here.**

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2023-08-09/143245f2-0e15-4c88-8182-93474c66864b/File.jpeg?tl_px=236,176&br_px=1096,657&force_format=png&width=560.0&wat_scale=50&wat=1&wat_opacity=0.7&wat_gravity=northwest&wat_url=https://colony-recorder.s3.us-west-1.amazonaws.com/images/watermarks/FB923C_standard.png&wat_pad=262,141)

**60. Click here.**

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2023-08-09/ba109e88-6273-4fec-9953-e380983a6f22/File.jpeg?tl_px=230,176&br_px=1090,657&force_format=png&width=560.0&wat_scale=50&wat=1&wat_opacity=0.7&wat_gravity=northwest&wat_url=https://colony-recorder.s3.us-west-1.amazonaws.com/images/watermarks/FB923C_standard.png&wat_pad=262,144)

**61. Click here.**

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2023-08-09/44373b98-caf1-4f77-9da4-4cfb2ac696e4/File.jpeg?tl_px=255,176&br_px=1115,657&force_format=png&width=560.0&wat_scale=50&wat=1&wat_opacity=0.7&wat_gravity=northwest&wat_url=https://colony-recorder.s3.us-west-1.amazonaws.com/images/watermarks/FB923C_standard.png&wat_pad=262,140)

**62. Click here, ensuring three correct volumes are selected.**

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2023-08-09/0461c402-c222-4e6e-aedd-419ecc8947bc/File.jpeg?tl_px=112,0&br_px=971,480&force_format=png&width=560.0&wat_scale=50&wat=1&wat_opacity=0.7&wat_gravity=northwest&wat_url=https://colony-recorder.s3.us-west-1.amazonaws.com/images/watermarks/FB923C_standard.png&wat_pad=262,39)

**63. 
Let's proceed to define the Initial Conditions, focusing only on the necessary and appropriate ones. To begin, we will set up the air flow over the IC. Click on "Initial conditions" to proceed with this step.**

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2023-08-09/43e15c0d-3054-4b20-9a87-4453b711edee/File.jpeg?tl_px=0,140&br_px=859,621&force_format=png&width=560.0&wat_scale=50&wat=1&wat_opacity=0.7&wat_gravity=northwest&wat_url=https://colony-recorder.s3.us-west-1.amazonaws.com/images/watermarks/FB923C_standard.png&wat_pad=66,138)

**64. Click "(U) Velocity"**

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2023-08-09/8bf23631-d335-455a-9320-4375d7d45a14/File.jpeg?tl_px=0,176&br_px=859,657&force_format=png&width=560.0&wat_scale=50&wat=1&wat_opacity=0.7&wat_gravity=northwest&wat_url=https://colony-recorder.s3.us-west-1.amazonaws.com/images/watermarks/FB923C_standard.png&wat_pad=76,158)

**65. In this step, we will define the air velocity solely in the Z-direction (the direction along which the IC is placed). We'll assume that there is no air flow in the other directions, and it remains stagnant. So Ux and Uy will be zero.**

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2023-08-09/92d54751-ef54-44d2-9583-23687822a006/File.jpeg?tl_px=62,0&br_px=922,480&force_format=png&width=560.0&wat_scale=50&wat=1&wat_opacity=0.7&wat_gravity=northwest&wat_url=https://colony-recorder.s3.us-west-1.amazonaws.com/images/watermarks/FB923C_standard.png&wat_pad=262,133)

**66. Type "0.3", this will be velocity of air in Z-direction. This value based on some standards which define the flow of air within a room.**

**67. Click here to apply the condition.**

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2023-08-09/b27397fc-ee84-4024-8350-ea822da0136b/File.jpeg?tl_px=129,0&br_px=988,480&force_format=png&width=560.0&wat_scale=50&wat=1&wat_opacity=0.7&wat_gravity=northwest&wat_url=https://colony-recorder.s3.us-west-1.amazonaws.com/images/watermarks/FB923C_standard.png&wat_pad=262,30)

**68. We need to set the initial temperature. Click on "(T) Temperature" to proceed with this task.**

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2023-08-09/771e811c-550a-49d3-acab-683794ebc7a6/File.jpeg?tl_px=0,92&br_px=859,573&force_format=png&width=560.0&wat_scale=50&wat=1&wat_opacity=0.7&wat_gravity=northwest&wat_url=https://colony-recorder.s3.us-west-1.amazonaws.com/images/watermarks/FB923C_standard.png&wat_pad=88,138)

**69. Adjust the default value to "30," this indicates the ambient temperature in degrees Celsius. It is important to note that this value may vary depending on the temperature at your specific location. Therefore, please set the appropriate value based on the temperature recorded on the day of the thermal measurement activity.**

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2023-08-09/3b1bdeb7-35d8-40d7-a9fd-8bcab0bf9f4b/File.jpeg?tl_px=74,0&br_px=933,480&force_format=png&width=560.0&wat_scale=50&wat=1&wat_opacity=0.7&wat_gravity=northwest&wat_url=https://colony-recorder.s3.us-west-1.amazonaws.com/images/watermarks/FB923C_standard.png&wat_pad=262,61)

**70. Click here. For the current simulation, only two initial conditions are required as other parameters do not significantly influence the simulation results.**

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2023-08-09/a872a39d-ab00-4e72-a223-9ab2515be474/File.jpeg?tl_px=128,0&br_px=988,480&force_format=png&width=560.0&wat_scale=50&wat=1&wat_opacity=0.7&wat_gravity=northwest&wat_url=https://colony-recorder.s3.us-west-1.amazonaws.com/images/watermarks/FB923C_standard.png&wat_pad=262,36)

**71. Now, let's configure the boundary conditions by clicking on 'Boundary conditions'. Here, we will define the appropriate boundary conditions to accurately replicate the given problem statement. Since heat transfers from the source to the surroundings through natural convection, we will choose the natural heat convection model for this purpose. Here heat source is IC itself.**

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2023-08-09/72f1a563-6d59-48ee-bef2-289499e1f297/File.jpeg?tl_px=0,176&br_px=859,657&force_format=png&width=560.0&wat_scale=50&wat=1&wat_opacity=0.7&wat_gravity=northwest&wat_url=https://colony-recorder.s3.us-west-1.amazonaws.com/images/watermarks/FB923C_standard.png&wat_pad=64,139)

**72. Click "Natural convection inlet/outlet"**

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2023-08-09/d072e028-296f-45ec-afc1-90b3c1a875e0/File.jpeg?tl_px=0,153&br_px=859,634&force_format=png&width=560.0&wat_scale=50&wat=1&wat_opacity=0.7&wat_gravity=northwest&wat_url=https://colony-recorder.s3.us-west-1.amazonaws.com/images/watermarks/FB923C_standard.png&wat_pad=179,138)

**73. Unhide the flow region if it is hidden**

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2023-08-09/e829ad07-9358-47eb-81f1-9dec3317bf5a/File.jpeg?tl_px=506,38&br_px=1366,519&force_format=png&width=560.0&wat_scale=50&wat=1&wat_opacity=0.7&wat_gravity=northwest&wat_url=https://colony-recorder.s3.us-west-1.amazonaws.com/images/watermarks/FB923C_standard.png&wat_pad=523,138)

**74. Ensure the flow region is visible**

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2023-08-09/033d5e1e-a09f-4341-a981-4d8f2301a398/File.jpeg?tl_px=235,124&br_px=1095,605&force_format=png&width=560.0&wat_scale=50&wat=1&wat_opacity=0.7&wat_gravity=northwest&wat_url=https://colony-recorder.s3.us-west-1.amazonaws.com/images/watermarks/FB923C_standard.png&wat_pad=262,138)

**75. Select all 6 faces of flow volume by clicking each faces.**

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2023-08-09/cda3c36e-f82c-46eb-88eb-2b0e1d1ea859/File.jpeg?tl_px=482,71&br_px=1342,552&force_format=png&width=560.0&wat_scale=50&wat=1&wat_opacity=0.7&wat_gravity=northwest&wat_url=https://colony-recorder.s3.us-west-1.amazonaws.com/images/watermarks/FB923C_standard.png&wat_pad=262,138)

**76. Make sure that all six faces are selected in the 'Assigned Faces' section. Now, update the 'Ambient temperature' to match the initial temperature value; let's set it to 30.**

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2023-08-09/39263fde-47db-4d06-a028-6f94346e37f7/File.jpeg?tl_px=30,0&br_px=1013,549&force_format=png&width=560.0&wat_scale=50&wat=1&wat_opacity=0.7&wat_gravity=northwest&wat_url=https://colony-recorder.s3.us-west-1.amazonaws.com/images/watermarks/FB923C_standard.png&wat_pad=262,96)

**77. Click here.**

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2023-08-09/92872db9-8c6c-4ea7-abe4-3159375afe06/File.jpeg?tl_px=114,0&br_px=973,480&force_format=png&width=560.0&wat_scale=50&wat=1&wat_opacity=0.7&wat_gravity=northwest&wat_url=https://colony-recorder.s3.us-west-1.amazonaws.com/images/watermarks/FB923C_standard.png&wat_pad=262,33)

**78. Expand the "Advanced Concepts" drop-down menu to set the power loss boundary condition. In the current scenario, the heat sink of the Integrated Circuit (IC) will be considered as a heat source, even though it receives heat from the electronics inside the IC. This simplification is implemented to facilitate the simulation process.**

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2023-08-09/4506b78f-9bd4-432d-a44c-b84f91f21702/File.jpeg?tl_px=0,176&br_px=859,657&force_format=png&width=560.0&wat_scale=50&wat=1&wat_opacity=0.7&wat_gravity=northwest&wat_url=https://colony-recorder.s3.us-west-1.amazonaws.com/images/watermarks/FB923C_standard.png&wat_pad=14,160)

**79. Click "Power sources"**

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2023-08-09/fd0d51ee-0339-47f2-9773-25f2f0442681/File.jpeg?tl_px=0,176&br_px=859,657&force_format=png&width=560.0&wat_scale=50&wat=1&wat_opacity=0.7&wat_gravity=northwest&wat_url=https://colony-recorder.s3.us-west-1.amazonaws.com/images/watermarks/FB923C_standard.png&wat_pad=78,190)

**80. Click "Absolute power source"**

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2023-08-09/7bcd368f-bc27-4cae-96da-eadb6e15fdef/File.jpeg?tl_px=0,176&br_px=859,657&force_format=png&width=560.0&wat_scale=50&wat=1&wat_opacity=0.7&wat_gravity=northwest&wat_url=https://colony-recorder.s3.us-west-1.amazonaws.com/images/watermarks/FB923C_standard.png&wat_pad=192,197)

**81. Enter the value "0.145" at "Power source value" for the power loss from the aluminum surface. Ensure unit is "W". This value is derived from the calculation we conducted earlier in the course.**

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2023-08-09/e6f3ef41-5f56-4d14-b4a0-4ad0af394b59/File.jpeg?tl_px=60,0&br_px=920,480&force_format=png&width=560.0&wat_scale=50&wat=1&wat_opacity=0.7&wat_gravity=northwest&wat_url=https://colony-recorder.s3.us-west-1.amazonaws.com/images/watermarks/FB923C_standard.png&wat_pad=262,92)

**82. Click "No Volumes assigned"**

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2023-08-09/73d7c43d-2f27-46c4-a74f-9e1222143184/File.jpeg?tl_px=24,31&br_px=884,512&force_format=png&width=560.0&wat_scale=50&wat=1&wat_opacity=0.7&wat_gravity=northwest&wat_url=https://colony-recorder.s3.us-west-1.amazonaws.com/images/watermarks/FB923C_standard.png&wat_pad=262,138)

**83. Click here to hide the flow region if it is not hidden.**

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2023-08-09/3c4e0b34-5921-4f1f-9a14-1988999175b6/File.jpeg?tl_px=506,29&br_px=1366,510&force_format=png&width=560.0&wat_scale=50&wat=1&wat_opacity=0.7&wat_gravity=northwest&wat_url=https://colony-recorder.s3.us-west-1.amazonaws.com/images/watermarks/FB923C_standard.png&wat_pad=517,138)

**84. Click on heat sink of IC**

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2023-08-09/5b881fcc-da06-4245-a592-676d4d24deef/File.jpeg?tl_px=506,51&br_px=1366,532&force_format=png&width=560.0&wat_scale=50&wat=1&wat_opacity=0.7&wat_gravity=northwest&wat_url=https://colony-recorder.s3.us-west-1.amazonaws.com/images/watermarks/FB923C_standard.png&wat_pad=306,138)

**85. Click here.**

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2023-08-09/4965c35a-cbbd-4b5c-9b30-5f15de384f44/File.jpeg?tl_px=118,0&br_px=977,480&force_format=png&width=560.0&wat_scale=50&wat=1&wat_opacity=0.7&wat_gravity=northwest&wat_url=https://colony-recorder.s3.us-west-1.amazonaws.com/images/watermarks/FB923C_standard.png&wat_pad=262,31)