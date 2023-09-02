
## Definition
**State Space** is the mathematical representation of the state of the system.
It refers to the set of possible states a system can be in.

A **system** can be a robot, a vehicle or any other entity that needs to navigate through the environment.

A **state** includes relevant variables that describe the system configuration (positions, velocities, 
orientations, etc).

- The state space describes the "*internal*" configuration of the system
- The map describes the "*external*" environment in which the system operates.


## State Spaces provided by OMPL

1. **RealVectorStateSpace:** This state space represents configurations as vectors of real numbers. It's often used for robots with continuous joints or systems with continuous parameters.
    
2. **SE2StateSpace:** This state space is designed for 2D rigid body motion planning. It represents configurations using (x, y) coordinates for translation and a single angle for rotation.
    
3. **SE3StateSpace:** Similar to SE2StateSpace, this state space is used for 3D rigid body motion planning. It represents configurations using (x, y, z) coordinates for translation and three angles (roll, pitch, yaw) for rotation.
    
4. **SO2StateSpace:** This state space represents rotations in 2D using a single angle. It's suitable for planar rotations.
    
5. **SO3StateSpace:** This state space represents rotations in 3D using quaternion representations or other rotation representations.
    
6. **CompoundStateSpace:** This state space allows you to combine multiple state spaces into a single compound state space. This is useful for planning problems involving robots with multiple components or different types of movements.
    
7. **DiscreteStateSpace:** This state space is for problems where the state can take on a finite number of discrete values. It's often used for grid-based planning or problems with a finite set of options.
    
8. **SubspaceStateSpace:** This state space is a subspace of another state space. It allows you to work with a subset of the dimensions of a larger state space.
    
9. **TimeStateSpace:** This state space is used to represent the passage of time. It's useful for planning problems that involve time-dependent actions.
    
10. **Custom State Spaces:** OMPL is highly customizable, and you can define custom state spaces tailored to your specific needs. This can be especially useful for representing complex robotic systems with unique configurations.