# SDDP Project

This project implements a Stochastic Dual Dynamic Programming solution for a cascaded hydroelectric reservoir optimization problem. The model was implemented without the SDDP library to gain a better understanding of how multistage stochastic optimization and the iterative generation of cuts function.

## Problem Context

Following a geothermal station failure, this model manages the water levels of three cascaded lakes (Lake 1 to Lake 2 to Lake 3). The objective is to minimize the total expected cost, which includes:

- **Power Purchase Costs:** Buying electricity from the neighboring grid when hydro production falls short.

- **Flood Penalties:** Costs incurred when lake levels exceed their maximum volume.

- **Safety Constraints:** Maintaining volumes above minimum levels and preventing game over scenarios by staying below critical levels.

## Structure

The notebook sddp_project.ipynb follows this order:

1. **Training**: SDDP algorithm training. The training logs (training_logs.txt) include extra iterations to ensure stable convergence with sufficient margin.
2. **Test**: Validation scenario execution.
3. **Visualization**: Generation of analysis plots.
4. **Explanations**: Detailed discussion of results and strategy can be found at the end.

## Figures

All visualization figures can be found in the `figures/` folder.
