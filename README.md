# README

# Optical Depth Modeling with Varying Parameters

This repository contains a Python implementation for modeling optical depth as a function of observing frequency, emission angle (\(\theta\)), spectral index (\(p\)), electron column density (\(N_e\)), and magnetic field strength (\(B\)). The script uses physical principles to compute optical depth and visualize the results using Matplotlib.

## Features

1. **Multiple Parameter Variations**:
   - **Spectral Index (\(p\))**: Visualizes optical depth for various spectral indices.
   - **Emission Angle (\(\theta\))**: Computes and plots optical depth for different angles.
   - **Magnetic Field (\(B\))**: Explores optical depth as a function of the magnetic field strength.
   - **Electron Column Density (\(N_e\))**: Demonstrates the effect of varying \(N_e\) on optical depth.

2. **Parallel Computing**:
   - Uses Python’s multiprocessing to compute results efficiently for multiple parameter sets.

3. **Interactive and Informative Plots**:
   - Provides detailed plots with annotations, legends, and varying line widths for clarity.

## Installation

### Prerequisites
Ensure you have Python 3.8 or higher installed along with the following libraries:
- `numpy`
- `matplotlib`
- `scipy`

To install missing dependencies, run:
```bash
pip install numpy matplotlib scipy
```

## Usage

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/optical-depth-modeling.git
   cd optical-depth-modeling
   ```

2. Run the script:
   ```bash
   python optical_depth_model.py
   ```

3. View the generated plots showing the relationship between optical depth and frequency under different conditions.

## Code Structure

### Main Components

1. **`model_f` Function**:
   - Computes optical depth using input parameters such as frequency, angle, spectral index, electron density, and magnetic field.

2. **`compute_model_f` Function**:
   - Uses multiprocessing to parallelize computations for efficiency.

3. **Visualization**:
   - Four plots are generated:
     - Optical depth vs. frequency for varying \(p\).
     - Optical depth vs. frequency for varying \(\theta\).
     - Optical depth vs. frequency for varying \(B\).
     - Optical depth vs. frequency for varying \(N_e\).

### Example Configurations

Modify the parameter lists (`params_list`) in the `__main__` block to customize computations for your specific use case.

### Outputs

- Four separate plots saved or displayed interactively.
- Each plot includes:
  - Axes labels, legends, and a horizontal reference line at \(y = 1\).
  - Clear annotations explaining the parameter values.

## Parameters

- **Frequency (\(\nu\))**: Range from 100 MHz to 9 GHz.
- **Emission Angle (\(\theta\))**: Radians (e.g., 0.15 to 1.50).
- **Spectral Index (\(p\))**: E.g., \(p = 2.0\) to \(p = 7.0\).
- **Electron Column Density (\(N_e\))**: \(10^{16}\) to \(10^{19}\) \(\text{cm}^{-2}\).
- **Magnetic Field Strength (\(B\))**: Gauss, e.g., \(10\) to \(90\).



## Contributing

Feel free to open issues or submit pull requests for bug fixes, new features, or enhancements.


