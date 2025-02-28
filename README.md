# Sine-Wave-Surface

### **What is a Sine Wave Surface?**  
A **sine wave surface** is a three-dimensional surface generated using a sine function, which creates periodic wave-like patterns. It is often used in computer graphics, physics simulations, and mathematical modeling to represent natural wave phenomena such as water ripples, sound waves, and electromagnetic fields.

This surface exhibits **periodic oscillations**, meaning it has repeating peaks and troughs. The shape is determined by a mathematical equation that defines the height variations based on the x and z coordinates.

---

### **Explanation of the Equation**  

The equation used in your code is:

\[
y = a \sin(b \sqrt{x^2 + z^2})
\]

#### **Expanding it down:**
1. **\( y \) (Height of the Surface)**  
   - This represents the height (or displacement) of the surface at any given point \( (x, z) \).

2. **\( a \) (Amplitude of the Wave)**  
   - This controls the **maximum height** and **depth** of the wave.
   - In your code, `amplitude = 2`, meaning the wave oscillates between **+2 and -2**.

3. **\( b \) (Frequency of the Wave)**  
   - This determines how many oscillations occur over a given distance.
   - In your code, `frequency = 0.5`, which controls the **spread** of the waves.

4. **\( \sqrt{x^2 + z^2} \) (Radial Distance)**  
   - This represents the **distance from the center (0,0) in the x-z plane**.
   - The wave height at any point depends on how far it is from the center.

#### **How It Works in the Code:**
- For every point on the 3D plane (`x, z`), the equation computes `y`, creating a circular ripple effect, similar to water waves when a stone is dropped into a pond.
- The sine function ensures smooth periodic oscillations.
- As **time progresses**, the equation is updated dynamically (`time` variable in the animation), making the wave move outward like a ripple.

---

### **Visualization & Real-World Application**
- This type of wave pattern is **radially symmetric**, meaning it spreads out uniformly from the center.
- Used in **water simulations, heat wave propagation, sound wave modeling, and terrain generation**.
