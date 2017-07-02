# Open motion simulator protocol specification

Data that is sent to a platform is encapsulated into a UDP datagramm with the following structure:

Yaw | Pitch | Roll | Height
---|---|---|---
float (4 bytes) | float (4 bytes) | float (4 bytes) | float (4 bytes) 

## Fields

* Yaw - heading of the platrorm in degrees.  
  *Platform is considered have 0 yaw at startup.*
* Pitch - pitch of the platform in degress.  
  *Platform is considered to have 0 pitch at startup.*
* Roll - roll of the platform in degress.  
  *Platform is considered to have 0 roll at startup.*
* Height - height of the platfrom from the base height in meters.  
  *Platform is considered to have 0 height at startup.*

## Data types
**float** is a single-precision floating-point format ([IEEE 754](https://en.wikipedia.org/wiki/Single-precision_floating-point_format))
