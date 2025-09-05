---

# GG Path Algorithm

A Python implementation of a procedural path and room generation algorithm, designed for dungeon or map layouts with city-block style connections and tunable complexity.

## Features

- **Path and Room Generation**: Creates multiple paths (main and alternatives) between a start and end point, with rooms represented as nodes and hallways as edges.
- **Randomization**: Supports random position nudging (fuzzing) and random deletion of rooms and hallways for varied layouts.
- **Cross-Path Connections**: Connects alternative paths to the main path for grid-like or looped structures.
- **Orphan Cleanup**: Removes disconnected rooms and hallways to maintain valid paths.
- **Untangling**: Reduces edge crossings for clearer visualizations using force-based node adjustment.
- **Visualization**: Plots generated paths and rooms using matplotlib for easy inspection.

## Usage

1. Clone the repository.
2. Install dependencies:
   ```
   pip install -r requirements.txt
   ```
3. Run the Jupyter notebook `notebook.ipynb` to generate and visualize sample paths.

## Algorithm Overview

1. Generate main and alternative paths between start and end nodes.
2. Randomly nudge room positions.
3. Connect corresponding rooms between paths.
4. Randomly delete rooms and hallways.
5. Clean up orphaned nodes and edges.
6. Untangle the graph for better visualization.

## Customization

- Adjust path generation parameters, fuzzing intensity, deletion percentages, and untangling settings in the notebook.
- Change visualization styles via the `GraphStyle` class.

## License

MIT License

---
