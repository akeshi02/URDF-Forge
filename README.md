# URDF 3D Builder for Ignition Gazebo

A lightweight, standalone web-based visual editor designed for the rapid prototyping of robot models. This tool allows users to build 3D assemblies and export them directly to **Unified Robot Description Format (URDF)** specifically optimized for **Ignition Gazebo (Fortress)**.

## 🚀 Overview

This application provides a "What You See Is What You Get" (WYSIWYG) interface for robotics engineers. By abstracting the complex XML structure of URDF files into a visual 3D workspace, it enables quick iteration on link dimensions, joint placements, and sensor configurations.

## ✨ Key Features

* **Interactive 3D Viewport:** Built with **Three.js**, featuring a ROS-standard (Z-up) coordinate system and real-time visualizers.
* **Component Palette:**
    * **Links:** Create structural components using Box, Cylinder, or Sphere primitives.
    * **Joints:** Establish Revolute or Fixed connections with visual axis indicators.
    * **Sensors:** Drag-and-drop pre-configured sensors including **LiDAR, RGB Camera, IMU, GPS (NavSat),** and **Sonar**.
* **Live Kinematics:** An **Animate Mode** that allows you to preview joint movements and verify motion ranges before exporting.
* **Robust Editor Tools:**
    * **Robot Tree:** Hierarchical navigation of the robot's link/joint structure.
    * **History System:** Full Undo/Redo support (up to 60 steps).
    * **State Management:** Save and load your project via JSON to persist your work.
* **One-Click Export Suite:**
    * `robot.urdf`: The complete XML description including physics and plugins.
    * `launch.py`: A ROS 2/Ignition launch file for immediate simulation testing.
    * `mesa_setup.sh`: Environment configuration for GPU/Mesa compatibility.

## 🛠️ Technical Stack

* **Three.js:** 3D rendering and object manipulation.
* **Vanilla JavaScript (ES6+):** Application logic and URDF generation.
* **HTML5/CSS3:** Modern, dark-themed "IDE" interface.
* **Standalone:** Zero dependencies or installation required.

## 📖 How to Use

1.  **Create Links:** Drag geometry items from the left sidebar into the 3D scene.
2.  **Establish Joints:** Use the **+ Joint Connect** tool to select a Parent link followed by a Child link.
3.  **Configure Properties:** Select any object to adjust its dimensions, mass, inertia, or sensor settings in the **Inspector** panel.
4.  **Verify Motion:** Toggle **▶ Animate** to see your
