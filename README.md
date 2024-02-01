# M.tech-Project-Work
Conventional Micro-drilling operation on Nickel Chrome alloy 625 using simulation in Deform 3D software. Performing practical experiments to try and test various methods and cutting parameters is an expensive endeavour even if we ignore errors and measurement issues that arise during machining. Computer simulations on the other hand provide us with accurate results and measurements to the real world provided correct process models are used. Deform 3D is a powerful process simulation system designed to analyse complex manufacturing processes' three-dimensional (3D) flow.

# Why is micro-drilling essential for Inconel 625?
Steam turbine blades made of Nickel-Chrome alloy 625 (Inconel 625) operate in high-temperature environments, and efficient cooling is crucial to prevent overheating and maintain structural integrity. To achieve this, microdrilling is employed to create intricate cooling hole patterns on the blades. These holes allow cooling air to flow through the blades, extracting heat and preserving their mechanical properties, etc.

# Why is simulation necessary?
Simulation is a cost-effective tool that helps analyze complex systems and processes, finds issues early on, and reduces development costs. It reduces risks, optimizes designs, predicts system performance, and informs decisions, thus optimizing productivity. It speeds up development, helps professionals train safely, and explores "what-if" scenarios. Scientists use it to validate scientific concepts and study inaccessible environments.

# Major Challenges encountered during simulation work. 
### 1) Selecting a Simulation Software for Conventional Micro-Drilling.
At first, I was unsure which software to use. Some PhD students recommended ANSYS (Explicit Dynamics). Although we can build a workpiece model in ANSYS, I decided to use CATIA software to develop a complex Micro drill bit. To use the Micro drill bit model in ANSYS, I converted the CATIA model to an SRT.file. However, I later chose Deform 3D software as it is more compatible than ANSYS. Deform 3D is better suited for providing insights into material deformation, tool wear, and chip formation. 

### 2) Learning Conventional Micro drilling simulation in Deform 3D software.
There are two ways of learning. The first is by being told what to do and what not to do by someone else, based on their experience. The second is through trial and error, which requires more time and effort. In my case, I only had the second option available. It took me over two months to get started, as I was only given access to a computer with 8GB RAM and an Intel Core i7 model. Each simulation took over 16 hours to complete. However, after a few days, I received support from the Deform 3D team. They suggested using adaptive meshing, which involved selecting a specific region for machining in both the workpiece and micro-drill bit. While this approach was time-consuming, it reduced the simulation time to 13 hours.

### 3) Differences in Jhonson Cook and Modified Jhonson Cook algorithms over Nickel Chrome alloy 625 (Inconel 625) for simulation.

# Observations
1) The main cause of the rise in temperature, stress, etc., is the impact of feed rate.
2) The material model is crucial to the simulation process.
3) Due to adiabatic heating, increasing spindle speeds cause the temperature to rise and axial force on the tool to decrease.
4) The modified Johnson-Cook model gives acceptable results compared to the normal Johnson-Cook model. 

# Limitations
1) The size of the micro drill bit has a direct impact on the size of the workpiece. The size of the workpiece should be 20% to 50% larger than the size of the micro drill 
   bit for chip removal. Additionally, the rpm for chip removal should be high.
2) Due to tool translational motion, the entire deformed material moves along the -ve Z direction if the Velocity boundary condition of the workpiece is not fixed in the Z 
   direction.
3) We cannot notice the burr formation on the exit side if the workpiece's velocity boundary condition is fixed in the Z direction.
4) Large-sized workpieces can make adaptive meshing difficult. And the material removal from the workpiece is not visible to us.
5) If we select an elastic or elastoplastic material type, the simulation will take longer to run and chip removal will be more challenging.
6) Since Deform3D is primarily used to calculate values for stress, strain, temperature, and strain rate, we cannot expect the hole quality. 
7) Simulated objects are thought to be made of the ideal material, free of any strain-hardening elements or residual stresses. 

# Future Work
1) If the simulation work's results coincide with those of the experiment, we can use the simulation technique by changing the parameters, which is safer than the actual 
   work and less expensive.
2) Deform 3D software needs to be improved to detect chips in huge workpieces for the micro-drilling process.


