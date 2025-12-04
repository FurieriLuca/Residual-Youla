# Learning Locally Exponentially Stabilizing Policies via Residual Youla Dynamics around Linear State Feedback

This repository contains the code, figures, and animations associated with the paper:

> **“Learning Locally Exponentially Stabilizing Policies via Residual Youla Dynamics around Linear State Feedback”**  
> Luca Furieri :contentReference[oaicite:0]{index=0}  

The paper derives a **state-space characterization of all dynamic state-feedback controllers** that render an equilibrium of a nonlinear input-affine continuous-time system **locally exponentially stable**. Under a standard stabilizability assumption on the linearization, any such controller can be written as:
- a linear baseline controller \(u(t) = Kx(t)\) (designed on the linearization),  
- plus **free nonlinear controller dynamics** that are themselves locally exponentially stable in suitable coordinates.

Conversely, every controller constructed in this way is locally exponentially stabilizing. This yields a **residual policy class** where:
- stability is guaranteed by construction;  
- performance objective and learning algorithm remain unconstrained. :contentReference[oaicite:1]{index=1}  

The paper illustrates the approach on a **cart–pendulum obstacle-avoidance task**, showing improved performance compared with standard RL and residual-RL policy classes of comparable size. :contentReference[oaicite:2]{index=2}  

---

## Repository structure

Adapt the paths below to your actual layout if needed. A typical structure is:

```text
.
├── main.ipynb        # Main notebook
├── figures/                  # Static figures used in the paper
│   ├── fig1_tip_trajectory.png
│   ├── fig2_training_curves.png
│   └── ...
├── animation/                # Animations of the trained controllers
│   ├── youla_les_policy.mp4      # Proposed Youla-based locally exponentially stable (LES) policy
│   ├── residual_mlp.mp4          # Residual MLP baseline
│   ├── residual_lstm.mp4         # Residual LSTM baseline
│   ├── pure_mlp.mp4              # Pure MLP policy
│   ├── pure_lstm.mp4             # Pure LSTM policy
│   └── ...
└── README.md
