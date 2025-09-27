# Catering Robot Simulation with Path Planning and SLAM

This project simulates a catering robot navigating a grid environment using dynamic path planning (D* Lite) and performing Simultaneous Localization and Mapping (SLAM) with Fast SLAM. The robot is designed to deliver items to specific locations while avoiding obstacles in a simulated environment.

---

## Features

### 1. **Robot Simulation**
- Simulates a robot with components like wheels and a central disk.
- Defines actions such as moving forward, backward, turning, and stopping.
- Implements a finite state machine to control the robot's behavior.

### 2. **Path Planning**
- Utilizes the **D* Lite** algorithm for dynamic pathfinding.
- Handles obstacles and computes the shortest path to the goal.
- Visualizes the robot's path, obstacles, and environment.

### 3. **SLAM (Simultaneous Localization and Mapping)**
- Implements **Fast SLAM** using particle filters for localization and mapping.
- Tracks the robot's estimated and true positions over time.
- Saves SLAM data to CSV files for further analysis.

### 4. **Visualization**
- Plots the robot's path, obstacles, and SLAM results.
- Generates and saves simulation and SLAM plots for analysis.

---

## Project Structure

- **`catering_robot_final.ipynb`**: Main Jupyter Notebook containing the simulation, path planning, and SLAM implementation.
- **Environment Setup**: Installs required libraries like `box2d`, `RobotSim373`, and dependencies for SLAM.
- **Robot Building**: Defines the robot's physical structure and actions.
- **Path Planning**: Implements the D* Lite algorithm for dynamic pathfinding.
- **SLAM**: Implements Fast SLAM with particle filters for localization and mapping.
- **Visualization**: Generates plots for the robot's path, obstacles, and SLAM results.

---

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/your-repo/catering-robot.git
   cd catering-robot

2. pip install box2d
    pip install "git+https://github.com/bblais/RobotSim373" --upgrade
    pip install -r PythonRobotics/requirements/requirements.txt

3. !pip install -q condacolab
    import condacolab
    condacolab.install()

---

## Usage
- Open the Jupyter Notebook catering_robot_final.ipynb in your preferred IDE or Jupyter - environment.
- Run the cells sequentially to:
- Build the robot and environment.
- Simulate the robot's movement and path planning.
- Perform SLAM and save results.
- Visualize the robot's estimated and true positions.

---

## Outputs

### Simulation Plots:
    - Visualizes the robot's path, obstacles, and environment.
### SLAM Data:
    - Saves SLAM results to projectslamvaluesfinal3.csv.
### SLAM Plots:
    - Saves SLAM visualization plots in the newplots4 directory.

---

## How It Works

### 1. **Robot Simulation**
- The robot is built using components like wheels and a central disk.
- Actions such as moving forward, turning, and stopping are defined.

### 2. **Path Planning**
- The **D* Lite** algorithm dynamically computes the shortest path to the goal while avoiding obstacles.

### 3. **SLAM**
- **Fast SLAM** uses particle filters to estimate the robot's position and map the environment.

### 4. **Visualization**
- Plots the robot's path, obstacles, and SLAM results for analysis.

---

## Dependencies

- **Python 3.x**
- Libraries:
  - `box2d`
  - `RobotSim373`
  - `matplotlib`
  - `numpy`
  - `pandas`
  - `condacolab`

---

## Contributing

Contributions are welcome! Feel free to open issues or submit pull requests.

---

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.

---

## Acknowledgments

- [RobotSim373](https://github.com/bblais/RobotSim373) for robot simulation.
- [PythonRobotics](https://github.com/AtsushiSakai/PythonRobotics) for SLAM implementation.