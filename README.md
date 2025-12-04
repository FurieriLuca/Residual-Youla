# Learning Locally Exponentially Stabilizing Policies via Residual Youla Dynamics around Linear State Feedback

This repository contains the code, figures, and animations associated with the paper:

> **“Learning Locally Exponentially Stabilizing Policies via Residual Youla Dynamics around Linear State Feedback”**  
> Luca Furieri

The paper derives a **state-space characterization of all dynamic state-feedback controllers** that render an equilibrium of a nonlinear input-affine continuous-time system **locally exponentially stable**. Under a standard stabilizability assumption on the linearization, any such controller can be written as:
- a linear baseline controller \(u(t) = Kx(t)\) (designed on the linearization),  
- plus **free nonlinear controller dynamics** that are themselves locally exponentially stable in suitable coordinates.

Conversely, every controller constructed in this way is locally exponentially stabilizing. This yields a **residual policy class** where:
- stability is guaranteed by construction;  
- performance objective and learning algorithm remain unconstrained. 
The paper illustrates the approach on a **cart–pendulum obstacle-avoidance task**, showing improved performance compared with standard RL and residual-RL policy classes of comparable size. 


-----

## Animation

![Youla LES policy](animations/augmented_controller_animation_resized.gif)



----
## Training curves and comparisons
![Training curves](figures/training_curves_comparison_confidence.pdf)
![Comparisons](figures/tip_trajectories_comparison_no_shadows.pdf)
