
## Definition

**Space information** refers to a crucial component that provides information and settings related to the configuration space (C-space) and the motion planning problem being solved. It plays a central role in configuring and guiding the behaviour of OMPL's motion planners.

Space information includes:

1. **State Space:** Space information includes a definition of the state space, which describes the possible configurations or states of the robot or system you are planning motions for. This state space specifies the dimensions, types, and constraints of the state space.
   
2. **Validity Checking:** Space information also encompasses validity checking functions or mechanisms. These functions are used to determine if a given state in the state space is valid or if it collides with obstacles or violates other constraints. Validity checking is crucial for ensuring the safety of the planned motions.
   
3. **Control Space:** In addition to the state space, space information may also include information about the control space if you're dealing with continuous control inputs. The control space defines the set of possible control inputs or actions that can be applied to the system.
   
4. **Planner Settings:** Space information provides settings and parameters for the motion planning algorithm (planner). This includes information about the start state, goal state, and any additional constraints or criteria for the planning problem.

5. **Optimisation Objectives:** If you are interested in optimizing the planned path or trajectory, space information can include optimization objectives that guide the planner in finding paths that minimize or maximize certain criteria (e.g., path length, smoothness, clearance from obstacles).

6. **State Sampling:** Space information may include methods or strategies for sampling states in the state space. Effective state sampling is essential for the exploration of the state space by the planner.

7. **Motion Model:** If applicable, space information may also define the robot's motion model, which describes how the system evolves from one state to another when control inputs are applied.

