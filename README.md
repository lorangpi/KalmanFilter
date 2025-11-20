# Kalman Filter for 1D Drone Localization


This repository implements the full solution to a 1D Kalman Filter localization problem for a drone, following the specification from Comp 150 Probabilistic Robotics — Homework 1. The system models the drone’s horizontal motion using position and velocity as the state, applies linear state-space dynamics with process noise, and incorporates noisy GPS measurements through the standard Kalman update.

The repo includes:

The prediction step using the motion model derived from Newton’s laws, including wind-based acceleration noise.

The measurement update using a GPS sensor model with configurable noise and dropout probability.

Tools to visualize uncertainty using covariance ellipses and to examine how uncertainty grows over time in the absence of measurements.

An environment simulator that produces noisy state transitions and optionally fails to generate sensor readings.

Experiments that quantify expected localization error at different GPS failure probabilities, and tests involving motor commands that influence acceleration.

Overall, the code demonstrates how prediction, measurement, and control interact in a Kalman Filter, and includes small experiments exploring uncertainty evolution, sensor failure, and system dynamics.