# Measuring-attenuation-of-opticalfiber-skill-assessment1-ocn

## Measuring Attenuation of Optical Fiber Using Python

## INTRODUCTION
Optical fibers are used to transmit information in the form of light signals over long distances. Even though optical fibers are highly efficient, some signal loss occurs when light travels through the fiber. This reduction in signal strength is known as attenuation. Attenuation is an important parameter in fiber optic communication because excessive attenuation reduces communication quality and transmission distance. Measuring attenuation helps in analyzing the performance and efficiency of optical fibers. Python programming can be used to automate attenuation calculations quickly and accurately using mathematical formulas. 

---

## OBJECTIVE
The main objectives of this experiment are:  To understand attenuation in optical fibers
 To calculate attenuation using input and output power values
 To implement attenuation measurement using Python programming
 To analyze the performance of optical fiber communication

---

## Attenuation Formula
The attenuation of an optical fiber is calculated using the formula:
A = 10 log10(Pin / Pout)
Where:  A = Attenuation in decibels (dB)  Pin = Input Power  Pout = Output Power
If fiber length is considered, attenuation per kilometer is calculated as:
Where:
 α = Attenuation coefficient (dB/km)  L = Length of optical fiber in kilometers

---

## SOFTWARE REQUIRED
Google colab (Python IDE)

---

## PROCEDURE
1. Install Python 3.x on the system or open Google Colab in a web browser. 2. Import the required Python libraries such as:
1. math for mathematical calculations
2. matplotlib.pyplot for graph plotting
3. Enter the input optical power value (Pin) in milliwatts (mW). 4. Enter the output optical power value (Pout) in milliwatts (mW). 5. Apply the attenuation formula to calculate signal loss
6. Compute the attenuation value using Python programming. 7. Display the calculated attenuation in decibels (dB). 8. Store the input power, output power, and attenuation values for graphical analysis. 9. Generate a graph using matplotlib to visualize:
1. Input Power
2. Output Power
3. Attenuation
10. Analyze the graph to observe the reduction in signal strength. 11. Verify that as output power decreases, attenuation increases. 12. Conclude the experiment based on the obtained attenuation results.

---

## PROGRAM CODE
~~~
import math
import matplotlib.pyplot as plt
# Input values
input_power = float(input("Enter Input Power (mW): "))
output_power = float(input("Enter Output Power (mW): "))
# Calculate attenuation
attenuation = 10 * math.log10(input_power / output_power)
# Print result
print("\n--- Optical Fiber Attenuation Result ---")
print(f"Input Power : {input_power} mW")
print(f"Output Power : {output_power} mW")
print(f"Attenuation : {attenuation:.2f} dB")
# Graph data
parameters = ['Input Power', 'Output Power', 'Attenuation']
values = [input_power, output_power, attenuation]
# Plot graph
plt.figure(figsize=(6,4))
plt.bar(parameters, values)
# Labels and title
plt.title("Optical Fiber Attenuation Analysis")
plt.ylabel("Values")
# Show graph
plt.show()
~~~

---

## OUTPUT

<img width="702" height="621" alt="Screenshot 2026-05-17 203353" src="https://github.com/user-attachments/assets/365a9cb1-3926-48bb-a0a5-e87852c07f0f" />

---

## ADVANTAGES
 Simple and fast calculation
 Reduces manual errors
 Easy to implement  Useful for fiber optic analysis and testing

---

## APPLICATIONS
 Fiber optic communication systems
 Telecommunication networks
 Internet backbone infrastructure
 Optical sensor systems
 Cable testing and maintenance

---

## RESULT
The attenuation of the optical fiber was successfully calculated using Python programming based on the given input and output power values. 

---

## CONCLUSION
In this experiment, attenuation in optical fiber was studied and measured using Python programming. The attenuation value was calculated using input and output optical power values. Python provides an efficient and accurate method for attenuation analysis in optical fiber communication systems.
