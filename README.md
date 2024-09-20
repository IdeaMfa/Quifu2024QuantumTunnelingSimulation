# Quifu2024QuantumTunnelingSimulation
A Python simulation of the 1D time-dependent Schrödinger equation using the Crank-Nicolson method. Visualizes wave packet propagation and interaction with potential barriers through animated plots.

## Installation
Clone the repository and install the dependencies.

```bash
git clone https://github.com/IdeaMfa/Quifu2024QuantumTunnelingSimulation.git
cd Quifu2024QuantumTunnelingSimulation
$ sudo dnf install python3 (Or install it from the address: https://www.python.org/downloads/)
python -m pip install -U pip
pip install numpy
pip install scipy
pip install matplotlib
```

#Features
- Wavepacket Evolution: Simulates the time evolution of a Gaussian wavepacket.
- Potential Barriers: Includes potential barriers, allowing you to observe the effect of tunneling and reflection.
- Crank-Nicolson Scheme: Uses the Crank-Nicolson algorithm for stable time-stepping.
- Visualization: Animates the wavepacket's evolution over time.

#Requirements
- Python 3.x
- NumPy
- SciPy
- Matplotlib
- You can install the dependencies using pip:
```bash
python -m pip install -U pip
pip install numpy
pip install scipy
pip install matplotlib
```

# How It Works
1. Gaussian Wavepacket: A Gaussian wavepacket is initialized with a given wave vector and width.
2. Crank-Nicolson Method: The wavepacket's time evolution is computed using the Crank-Nicolson method, which ensures stability in the time-stepping process.
3. Potential Barriers: Two different simulations are run, each with varying potential barriers in the middle of the simulation domain.
4.Animation: The results are visualized as an animated plot, showing the absolute value of the wavefunction over time.

## Key Functions

- **`gaussian_wavepacket(x, x0, k, sigma)`**: Initializes a Gaussian wavepacket.
  
  - `x`: Spatial grid points.
  - `x0`: Center of the wavepacket.
  - `k`: Wave number (momentum).
  - `sigma`: Width of the wavepacket (optional, default is 0.1).

- **`CrankNicolson(psi0, V, x, dt, N)`**: Implements the Crank-Nicolson method to evolve the wavefunction in time.

  - `psi0`: Initial wavefunction (complex).
  - `V`: External potential array.
  - `x`: Spatial grid points.
  - `dt`: Time step for evolution.
  - `N`: Number of time steps (optional, default is 100).

# Running the Simulation
- To run the simulation, simply execute the script:
```bash
python schrodinger_simulation.py
```
This will display an animation of the wavepacket as it interacts with the potential barriers.

## Customization
You can modify parameters like the initial wave vector k, the potential height V, and the width of the wavepacket sigma to see different behaviors.

## Example Output
The animation produced by this code visualizes the propagation of two wavepackets through different potential barriers, showcasing effects like reflection and tunneling.

## License
This project is developed by Fatih Aytar (IdeaMfa) and is available as open source.
