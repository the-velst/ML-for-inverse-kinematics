# ML for Robotics: Inverse Kinematics

## Overview

This project solves the inverse kinematics problem of a 2-link robotic manipulator using Machine Learning.

Given:

(px, py)

Predict:

(θ1, θ2)

The same position can have multiple valid solutions (elbow-up / elbow-down).

We compare:

- Multi-Layer Perceptron (MLP)
- Normalizing Flows

---

## Why MLP Fails

MLP gives only one output for each input.

Since inverse kinematics may have multiple valid outputs, MLP often predicts an averaged solution.

---

## Why Normalizing Flows

Normalizing Flows learn the probability distribution of possible joint angles.

This allows the model to represent multiple valid IK solutions.

---

## Tech Stack

- Python
- TensorFlow
- NumPy
- Scikit-learn
- Jupyter Notebook

---

## Results

- MLP struggled in multi-solution cases
- Normalizing Flows handled multiple solutions better

---

## Future Scope

- Parallel Manipulators
- 3D Robot Arms
- Motion Planning
