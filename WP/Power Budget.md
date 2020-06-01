# WP2.4 Power Budget 

![![GitHub Logo](/image/logo.png)
Format: ![Alt Text](url)]

### Sat Energy Capacity Reports 

This is the OPA Report, OAP is the average orbit power. We assume that the sat is in SSO orbit, which mean that the sat is always in sun zone. We assume two that the satellite is only rotation on one axis relative to the sun. 


On the sat we have solar panel, on each face, to calculate the OAP, we want to know the average power that the solar panel will provide 

To do that's we need to calculate the average projected area of the sat during its rotation on its axis. 

The formula to calculate the exposed area is this one : 

### f(x) = cos(x)*A+sin(x)*B 

Where A and B are the area of the face and 'df the rotation of the sat (moving between 0 and 90'b0) 

And then we just want to calculate the average value of the function on interval (0;90) 
We first calculate the integrale and then divide it by delta of 'df(90) 

### f(x) = cos


And the result are : 

for A = 50cm2 and B = 50cm2 
P = (2*(100))/pi 
### = 63.66 cm2 


for A = 50cm2 and B = 100cm2 
P = (2*(150))/pi 
### = 95.4 cm2 

The first result if for the sat rotating with the big face on top (1)

The second result if for the sat rotating with a small face on top (2) 


Then we know that the area used by solar panel on face is about 70%, and that solar efficiency is about 25%. We finally know that the solar power received by the sat will be about 1300W.m2 = 0.13W.cm2 

OAP = (((Average projected area)*70%)*0.13)*25% 

OAP1 = ((63.66*70%)*0.13)*25% 
### OAP1 =  1.448W 

OAP2 = ((95.4*70%)*0.13)*25% 
### OAP2 = 2.170W 

As we always have sun a big capacity battery is not required 

Now it\'92s better to do the calculation with actual solar cell. We may use this one http://www.azurspace.com/images/0003429-01-01_DB_3G30C-Advanced.pdf\

Surface area = 30.18cm2 = 60% of the face area 
Efficiency = 28 % 

OAPreal1 = ((63.66*60%)*0.13)*28% 
### OAPreal 1 = 1.390W 

OAPreal2 = ((95.4*60%)*0.13)*28% 
### OAPreal2 = 2.083W 
