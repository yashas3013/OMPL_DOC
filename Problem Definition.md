
## Definition

**Problem definition** refers to a crucial component that specifies the details of the motion planning problem to be solved. It serves as a bridge between the motion planning algorithm (planner) and the specifics of the task you want to accomplish with OMPL.

1. **Start State:** The problem definition includes the specification of the start state of the robot or system. The start state represents the initial configuration from which the motion planning process begins.

2. **Goal State:** Similarly, the problem definition specifies the goal state, which represents the desired final configuration of the robot or system. The goal state defines what you want to achieve through motion planning.

3. **State Space:** The problem definition typically references the state space, which describes the possible configurations or states of the robot. The state space may have been previously defined as part of the space information.

4. **Validity Checking:** If needed, the problem definition may include information about how to perform validity checking on states to ensure they are collision-free and satisfy any other constraints. Validity checking is crucial for avoiding obstacles and ensuring safe motion planning.

5. **Optimization Objectives:** In some cases, the problem definition specifies optimization objectives, which guide the planner in finding paths or trajectories that optimize certain criteria (e.g., path length, smoothness, clearance from obstacles).
    
6. **Other Constraints:** Depending on the specific motion planning problem, the problem definition may include additional constraints or criteria that must be satisfied during the planning process.
    
7. **Other Parameters:** The problem definition can include other parameters or settings that are specific to the particular motion planning problem you are solving.


## Difference Between Problem Definition and Space information

1. **Space Information:** Space information primarily focuses on defining the characteristics of the state space in which the motion planning problem is formulated. It includes information about the state dimensions, types, constraints, validity checking, and often the control space if continuous control inputs are involved. Space information is a fundamental component for motion planners to understand the structure of the state space and how to sample, validate, and navigate within it. It serves as the mathematical foundation for the planning process.
    
2. **Problem Definition:** The problem definition, on the other hand, specifies the particular instance of the motion planning problem you want to solve using OMPL. It includes details such as the start state, goal state, optimization objectives (if any), additional constraints, and other problem-specific parameters. The problem definition is a higher-level component that builds upon the space information. It defines the specific task or goal within the state space and guides the planner to find a solution that satisfies these task-specific requirements.