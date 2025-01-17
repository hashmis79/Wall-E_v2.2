## LSA - Light Sensor Array

### Components of LSA
| Component   | Description   | Quantity |
| ----------- | ------------- | -------- |
| LED         | Emits light   |  4       |
| PhotoDiode  | Absorbs light |  4       |
| IC LM324    | Op.Amp. IC    |  1       |  
| Resistors   | Limit Current |  8       |

### Function of Components
- LED
	- LSA consists of Four LED and PhotoDiode Pairs. The specific LED's emit IR light which is incident on the surface and some of it is absorbed by the surface. The voltage source For the LEDs to glow is VCC.

- PhotoDiode
	- Based upon the reflectivity coefficient of the surface( generally greater than 1), the remaining light reflected from the surface is captured by the Photodiodes. IR light LEDs and complimentary photodiodes are used to efficiently detect the surface (white/black line) as the environment also contains unwanted light for the LSA sensor. The amount of light received is directly proportional to the current generated by it. More the light, more the current, more the reading.
 
- IC LM324 
	- This is a Quad(4) OP.Amp. IC. Op.Amp i.e Operation Amplifiers amplify the current with constant volatge. Since the current reading from photo diodes is significantly small and difficult to compare, it needs to be amplified. The 4 amplified outputs serve as raw readings of LSA.

- Resistors
	- Now to limit the current and thus to protect the LEDs, PhotoDiodes current limiting resistors are used.

### Working Principle
- LSA works on the principle of reflectivity of light for different types of surfaces.
	- Black Surface -> HIGH absorptivity -> LESS reflectivity
	- White Surface -> LOW absorptivity -> HIGH reflectivity
	
### Applications 
- Application of LSA majorly lies in line following.

### Scope of Improvement
- LSA sometimes provides slightly inaccurate readings due to external light and conditions. Therefore, LSA has low accuracy. Hence LSA should be kept close to the ground.
- As of now only white and black surfaces are being mapped. Given accurate sensors and proper mapping we can map LSA for any range of RGB colours.

