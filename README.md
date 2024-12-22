# FermentDynamics
FermentDynamics is a Python-based simulation tool designed to model the evolution of bacterial populations during the fermentation process, specifically tailored for sourdough or pizza dough. The project leverages mathematical models like the Ratkowsky growth model and integrates environmental factors such as temperature and pH dynamics to predict the optimal conditions for fermentation.

## Features

- **Simulates bacterial population growth** for key microbes:
  - Lactic acid bacteria
  - Acetic acid bacteria
  - Succinic acid bacteria
  - Gluconic acid bacteria
- **Models pH evolution** during fermentation.
- Accounts for the effect of **temperature schedules** and **pH inhibition** on growth.
- Implements the **Ratkowsky model** for temperature-dependent growth rates.
- Interactive visualizations of bacterial dynamics and pH shifts.

## Installation

Clone this repository and install the necessary Python packages:

```bash
# Clone the repository
git clone https://github.com/yourusername/FermentDynamics.git

# Navigate to the project directory
cd FermentDynamics

# Install dependencies
pip install -r requirements.txt
```

## Usage

### Running the Simulation

To run the fermentation simulation, simply execute the main script:

```bash
python simulate.py
```

You can customize parameters such as initial bacterial populations, temperature schedules, and pH levels in the script.

### Interactive Visualization

Use the interactive notebook for dynamic exploration of the model:

```bash
jupyter notebook interactive_simulation.ipynb
```

Adjust parameters like temperature, pH, or acidification rate (`alpha`) to see their effects on bacterial dynamics and pH evolution.

## Example Output

### Population Dynamics

![Bacterial Growth](example_growth.png)

### pH Evolution

![pH Shift](example_pH.png)

## Project Structure

```plaintext
FermentDynamics/
├── README.md              # Project documentation
├── simulate.py            # Main simulation script
├── interactive_simulation.ipynb # Jupyter notebook for interactive visualization
├── models.py              # Mathematical models and differential equations
├── requirements.txt       # List of dependencies
├── examples/              # Example scripts and output images
└── tests/                 # Unit tests for the simulation
```

## Models Used

1. **Ratkowsky Model**: Describes temperature-dependent bacterial growth rates.
2. **pH Inhibition**: Incorporates pH-dependent growth limitations.
3. **Logistic Growth**: Models competition for resources using a carrying capacity.

## Contributing

Contributions are welcome! Please fork the repository and submit a pull request. For major changes, open an issue first to discuss your ideas.

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.

## Acknowledgments

- Inspired by research on microbial fermentation dynamics.
- Special thanks to the open-source community for tools like NumPy, SciPy, and Matplotlib.
