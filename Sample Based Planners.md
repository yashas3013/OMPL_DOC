

## Definition
**Sample-based planners** is to explore the configuration space by randomly or systematically sampling points in the space and then connecting these points to form a feasible path from the start to the goal configuration.

1. **Representation of Space:**
    
    - **Sample-Based Planner:** Sample-based planners work with a representation of the configuration space (C-space) that consists of individual points (samples) randomly or systematically placed in the space. These samples are connected to form a graph or tree structure that represents possible paths.
    - **Grid-Based Planner:** Grid-based planners discretize the C-space into a grid of cells. Each cell represents a distinct configuration, and the entire grid collectively represents the C-space. These grids are often referred to as occupancy grids or costmaps.
2. **Complexity of Environments:**
    
    - **Sample-Based Planner:** Sample-based planners are well-suited for high-dimensional and complex C-spaces with irregular shapes, obstacles, or narrow passages, where a grid-based approach may suffer from an exponential increase in the number of cells.
    - **Grid-Based Planner:** Grid-based planners are better suited for relatively structured and low-dimensional environments, where the C-space can be discretized with a reasonable number of cells without excessive memory and computational requirements.
3. **Memory Usage:**
    
    - **Sample-Based Planner:** Sample-based planners typically use less memory compared to grid-based planners since they only store a subset of sampled configurations and their connections in the C-space.
    - **Grid-Based Planner:** Grid-based planners require memory to store the entire grid, which can be memory-intensive, especially in high-dimensional spaces or when high-resolution grids are used.
4. **Efficiency and Search Strategy:**
    
    - **Sample-Based Planner:** Sample-based planners use techniques like random sampling (e.g., RRT) or systematic sampling (e.g., PRM) combined with nearest-neighbor searches to explore the C-space efficiently. They often focus on exploring regions of the space where solutions are more likely to be found.
    - **Grid-Based Planner:** Grid-based planners rely on grid-based search algorithms like A* or Dijkstra's algorithm to search through the grid cells. These planners may perform well in grid-like environments but may struggle with high-dimensional spaces or intricate configurations.
5. **Collision Checking:**
    
    - **Sample-Based Planner:** Collision checking is performed for sampled configurations and their connections. This allows sample-based planners to quickly reject infeasible paths and explore promising areas of the C-space.
    - **Grid-Based Planner:** Collision checking is done for each grid cell, which can be computationally expensive, especially in high-resolution grids.
6. **Flexibility:**
    
    - **Sample-Based Planner:** Sample-based planners are more flexible in handling complex and changing environments because they adapt to the distribution of obstacles through sampling.
    - **Grid-Based Planner:** Grid-based planners require a predefined grid structure, which may need to be recomputed if the environment changes significantly.