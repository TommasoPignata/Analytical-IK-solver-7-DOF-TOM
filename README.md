# Analytical-IK-solver-7-DOF-TOM
A closed-form inverse kinematics solver for 7-DOF anthropomorphic
(shoulder–elbow–wrist) robot arms, packaged for ROS2.

Unlike numerical solvers, it returns all solution branches
deterministically, with no seed pose, no convergence failures, and
bounded computation time making it suitable for real-time servo and
force control loops.

**Status:** validated on KUKA hardware.
Includes URDF-to-DH extraction so it runs on any arm whose DH table
correctly describes it.

## Demos

### Arm-angle decoupling with target pose
Shows the redundancy parameter being varied independently of the
end-effector pose — the arm sweeps through its null space while the
tool frame stays fixed.

### Control-mode transitions
Position control → servo-mode null-space exploration → force-controlled
obstacle interaction, without re-planning or leaving the solution branch.

https://github.com/user-attachments/assets/77933ecc-79b5-467a-ac12-f3f8fc5ff067

Eߣ�B��B��B�B�B��matroskaB��B��S�g
