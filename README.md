# SubwaySurferModelgame

## Overview
This repository contains the packaged Windows 64-bit build of a high-speed endless runner, featuring lane-switching mechanics and dynamic obstacle avoidance. Developed using Unreal Engine, the project prioritizes responsive input handling and optimized real-time rendering.

## Technical Architecture
While the core loop is gameplay-focused, the underlying architecture emphasizes stability, performance, and version control best practices:
* **Engine:** Unreal Engine (Win64 build)
* **Performance Profiling:** Assets and draw calls have been optimized to ensure a stable frame rate without VRAM overflow.
* **Version Control:** Project source is managed via Git, utilizing strict feature branching and Git LFS (Large File Storage) to handle heavy binary assets seamlessly across local and cloud environments.

## Installation & Execution
This repository houses the standalone compiled build. No engine installation or IDE is required to run the game.

1. Clone the repository to your local Windows machine.
2. Ensure the directory structure remains intact.
3. Double-click `SubwaySurfersUpload.exe` to launch the application.

## Directory Structure
* `/Engine/` — Contains the required Unreal Engine runtime binaries and dependencies.
* `/SubwaySurfersUpload/` — Contains the packaged game content, including baked textures, models, and audio.
* `Manifest_NonUFSFiles_Win64.txt` — The build manifest file detailing non-unreal file system dependencies.
* `SubwaySurfersUpload.exe` — The primary executable.

## Development Workflow
This project utilizes a continuous integration mindset with a strict branching strategy to prevent merge conflicts and broken builds:
* `main`: Protected branch containing only stable, reviewed releases.
* `development`: The primary integration branch for ongoing work.
* `feature/*`: Dedicated branches for independent script modifications and asset optimization.
