# RandomWalkVisualizer

## Description
This Python script simulates a 2D random walk, where a particle moves in one of four directions (up, down, left, right) with equal probability at each step. It visualizes the path using `matplotlib`, featuring a gradient colormap to indicate the progression of steps over time. The plot highlights the starting and ending points and is saved as a high-quality PNG image. Optionally, an animation can be enabled to show the path's evolution step-by-step. The script uses `numpy` for efficient array operations.

## Features
- Simulates a 2D random walk with customizable step count and step size.
- Visualizes the path with a gradient colormap to show temporal progression.
- Marks the starting (green) and ending (red) points of the walk.
- Saves the plot as a high-quality PNG file (`random_walk_plot.png`).
- Supports optional animation to visualize the walk's progression.
- Displays the final distance from the origin in the plot title.
- Uses vectorized operations for improved performance and scalability.

## Requirements
- Python 3.x
- Required libraries:
  - `numpy`
  - `matplotlib`
- Optional (for saving animation as GIF):
  - `pillow` (for `Pillow` writer)
  - `imagemagick` (alternative for GIF export)

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/random-walk-visualizer.git
   ```
2. Navigate to the project directory:
   ```bash
   cd random-walk-visualizer
   ```
3. Install the required libraries:
   ```bash
   pip install numpy matplotlib
   ```
4. (Optional) For GIF animation support, install `pillow`:
   ```bash
   pip install pillow
   ```

## Usage
1. Save the script as `random_walk.py`.
2. Run the script:
   ```bash
   python random_walk.py
   ```
3. The script will:
   - Simulate a 2D random walk (default: 1000 steps).
   - Generate a static plot of the path with a gradient colormap, marking the start (green) and end (red) points.
   - Save the plot as `random_walk_plot.png` in the project directory.
   - Display the plot.
4. To enable animation, modify the script to call `random_walk_2d(animate=True)`. Optionally, uncomment the GIF saving line to export the animation as `random_walk_animation.gif`.

## Example Output
Below is an example of the static plot for a 1000-step random walk:

![Random Walk Plot](random_walk_plot.png)

*(Note: Add a screenshot of the plot by running the script and uploading the generated PNG file to the repository.)*

## Code Explanation
- **Function**: `random_walk_2d(num_steps=1000, step_size=1.0, animate=False)`
  - Simulates a 2D random walk with specified number of steps and step size.
  - Uses `numpy` for efficient path storage and random direction generation.
  - Generates a static plot with a gradient colormap or an animated plot if `animate=True`.
  - Saves the plot as `random_walk_plot.png`.
- **Key Parameters**:
  - `num_steps = 1000`: Number of steps in the random walk.
  - `step_size = 1.0`: Size of each step.
  - `animate = False`: If True, displays an animated plot instead of a static one.

## Contributing
Contributions are welcome! Please follow these steps:
1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Make your changes and commit (`git commit -m 'Add new feature'`).
4. Push to the branch (`git push origin feature-branch`).
5. Create a pull request.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contact
For questions or feedback, feel free to open an issue on GitHub or contact [your-email@example.com](mailto:your-email@example.com).