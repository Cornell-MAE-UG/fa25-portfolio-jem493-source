---
layout: default
title: "Small-Scale Wind Turbine Design"
collection: projects
---

## Overview
For the MAE 4272 (Fluids Laboratory) Course, our team was tasked with designing a small-scale wind turbine blade to maximize power extraction within specific constraints. The objective was to engineer a practical blade geometry capable of withstanding realistic operating loads while adhering to a 2000 RPM safety limit and a maximum torque braking power of 3.5 N-cm. The final design was validated through experimental testing in the "Big Blue" wind tunnel in the Upson fluid dynamics lab.

## Design Process
Our design strategy prioritized aerodynamic performance and structural integrity.
* **Optimization:** We utilized a Weibull probability distribution to identify the optimal design wind speed of 5.3 m/s, ensuring we targeted the highest energy density area of the wind curve to maximize the efficiency and power generation of our turbine blade.
* **Aerodynamics:** We selected the NACA4412 airfoil for its good performance characteristics across a range of conditions. Using element-wise analysis in MATLAB, we optimized the blade geometry, settling on a 90-degree angle of twist and a taper ratio of 3.25 to reduce the blade mass while maintaining lift throughout.
* **Fabrication:** The blades were modeled in CAD to ensure compatibility with the 3D printing process and the hub connector constraints. The 3D printing was outsourced (for all groups) with the assistance of course staff.

<figure style="text-align: center;">
  <img src="{{ '/assets/blade-cad-2.jpg' | relative_url }}" alt="CAD rendering" style="width: 100%; max-width: 600px;">
  <img src="{{ '/assets/Blade-CAD.jpg' | relative_url }}" alt="CAD Dimensions" style="width: 100%; max-width: 600px;">
  <figcaption><em>Figure 1: CAD rendering of the final blade geometry and dimensions.</em></figcaption>
</figure>

## Testing Summary
We validated the design in the wind tunnel across wind speeds corresponding to free-spin rotational rates of 250–550 RPM. We applied incremental electrical loading to the torque brake to characterize performance until stall.
* **Results:** The turbine achieved a maximum power output of **1.1 W** at 400 RPM.
* **Analysis:** Peak efficiency occurred at a tip-speed ratio (TSR) of 0.51. This was lower than our theoretical model, likely due to low Reynolds number effects during the tunnel test which reduced the performance of the airfoils.

<figure style="text-align: center;">
  <img src="{{ '/assets/power-curve.jpg' | relative_url }}" alt="Power Curve" style="width: 100%; max-width: 600px;">
  <figcaption><em>Figure 2: Experimental power curves showing peak performance at various RPMs. This data was collected using a LabView VI prebuilt in the Big Blue wind tunnel.</em></figcaption>
</figure>

## My Contribution
In this group project, I focused primarily on developing the MATLAB code to calculate the Weibull distribution and optimal twist/taper ratios. We had group members who have taken the MAE wind power class, which proved very helpful in refining and applying concepts introduced during this class.
