# WP2.4 Power Budget 

### Sat Energy Capacity Reports 

This is the OPA Report, OAP is the average orbit power. We assume that the sat is in SSO orbit, which mean that the sat is always in sun zone. We assume two that the satellite is only rotation on one axis relative to the sun. 

![](/WP/image/sketch2.png) 


(Click on the image the see the actual simulation of the SSO orbit) 

[![Alt text](https://img.youtube.com/vi/RoKZx84o4Kk/0.jpg)](https://www.youtube.com/watch?v=RoKZx84o4Kk)

On the sat we have solar panel, on each face, to calculate the OAP, we want to know the average power that the solar panel will provide 

To do that's we need to calculate the average projected area of the sat during its rotation on its axis. 

The formula to calculate the exposed area is this one : 

### f(x) = cos(x)*A+sin(x)*B 

Where A and B are the area of the face and 'df the rotation of the sat (moving between 0 and 90°) 

And then we just want to calculate the average value of the function on interval (0;90) 
We first calculate the integrale and then divide it by delta of x (90) 

### f(x) = ∫(A*sin(x)+B*cos(x),x,0,π/2)/(π/2-0)

### = (2 (A + B))/π

And the result are : 

for A = 50cm2 and B = 50cm2 
P = (2*(100))/pi 
### = 63.66 cm2 


for A = 50cm2 and B = 100cm2 
P = (2*(150))/pi 
### = 95.4 cm2 

The first result if for the sat rotating with the big face on top (1)

The second result if for the sat rotating with a small face on top (2) 

![](/WP/image/cube.png)


Then we know that the area used by solar panel on face is about 70%, and that solar efficiency is about 25%. We finally know that the solar power received by the sat will be about 1300W.m2 = 0.13W.cm2 

OAP = (((Average projected area)*70%)*0.13)*25% 

OAP1 = ((63.66*70%)*0.13)*25% 
### OAP1 =  1.448W 

OAP2 = ((95.4*70%)*0.13)*25% 
### OAP2 = 2.170W 

As we always have sun a big capacity battery is not required 

Now it\'92s better to do the calculation with actual solar cell. We may use this one http://www.azurspace.com/images/0003429-01-01_DB_3G30C-Advanced.pdf

Surface area = 30.18cm2 = 60% of the face area 
Efficiency = 28 % 

OAPreal1 = ((63.66*60%)*0.13)*28% 
### OAPreal 1 = 1.390W 

OAPreal2 = ((95.4*60%)*0.13)*28% 
### OAPreal2 = 2.083W 

The next part was the orbit / eclipse simulation 
A 97° SSO Orbit have been simulated 

During the year the % of available power is evoluting between 75% and 100% 
the worst time is summer and the best time is winter. 

![](/WP/image/chart-3.png) 

Wich mean the the worst case of the worst case is 75% of 1.390 = 1.0425W
The best case of the worst case is 1.390W 

The worst case of the best case is 75% of 2.083W = 1.562W 
The best case of the best case is 2.083W


