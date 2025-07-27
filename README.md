# Smart Grid Energy Allocation using Genetic Algorithm

## Overview
This project implements a Genetic Algorithm (GA) and a Greedy Algorithm to optimize energy allocation in a smart grid environment. The goal is to minimize the total cost of energy supply while satisfying demand, respecting source capacities, and considering line losses.

## Features
- Flexible data loading from CSV files
- Customizable GA parameters (population size, generations, mutation rate)
- Serial and parallel GA implementations
- Multiple constraints: demand satisfaction, source capacity, energy wastage, and line loss
- Greedy algorithm for baseline comparison
- Visualization of convergence, CPU usage, execution time, allocation heatmaps, and cost improvement

## File Structure
- `GA_Final.ipynb`: Main Jupyter notebook with all code, experiments, and plots
- `dataset.csv`: Input data file (demand, capacity, cost)
- `README.md`: Project documentation (this file)

## How to Run
1. Open `GA_Final.ipynb` in Jupyter Notebook or VS Code.
2. Ensure `dataset.csv` is present in the same directory.
3. Run all cells to execute the algorithms and generate plots.
4. Adjust GA parameters in the main block as needed.

## Genetic Algorithm Details
- **Chromosome Encoding**: Each chromosome is a flattened array representing energy allocations for all nodes, sources, and hours.
- **Fitness Function**: Penalizes unmet demand, energy wastage, capacity violations, and excessive line loss. Lower fitness is better.
- **Selection**: Tournament selection.
- **Crossover**: Single-point crossover.
- **Mutation**: Random value mutation and swap-based mutation for diversity.
- **Parallelization**: Fitness evaluation can be parallelized using threads.

## Visualization
- Fitness score convergence
- CPU usage per generation
- Execution time comparison
- Cost improvement over greedy baseline
- Allocation heatmaps and cost vs demand plots

## Requirements
- Python 3.x
- numpy
- pandas
- matplotlib
- seaborn
- psutil

Install requirements with:
```
pip install numpy pandas matplotlib seaborn psutil
```

## Customization
- Change GA parameters (`population_size`, `generations`, `mutation_rate`) in the main block.
- Modify the fitness function to add or remove constraints as needed.

## License
This project is for academic and educational use.

## Contact
For questions or suggestions, please contact the project maintainer.
