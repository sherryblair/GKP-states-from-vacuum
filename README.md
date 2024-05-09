Optimization to find non-linear optical circuits preparing target GKP states.

The notebook "GKP states from vacuum.ipynb" contains commented code using a truncated Fock representation to optimize circuits of displacements, squeezers and Kerr gates so as to maximize the fidelity of the output with a target (single-mode) GKP state. The input is the vacuum state.

We use the Strawberry Fields software to simulate the action of the circuit on a photonic quantum computer, and for the optimization we use the built-in algorithms of scipy.optimize. We calculate the Glancy-Knill error probability (https://journals.aps.org/pra/abstract/10.1103/PhysRevA.73.012325) for our generated GKP states.

To change the target state, just change the angles in the "state" variable of the "cooled_squared_vac_overlap" function (see also Strawberry Fields documentation).
