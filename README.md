# ActivityTaskManagerServiceTutorial

This project demonstrates the **Activity Task Manager Service** in Android. It showcases how activities are launched, managed in tasks, and handled across different launch modes (`standard`, `singleTop`, `singleTask`). It illustrates the system's decision to reuse or recreate activity instances within tasks.

## Concepts
- **Activity Task Manager Service**: Manages activity launches, task stacks, and process creation. It ensures that activities are created or reused based on system requirements.
- **IPC (Inter-Process Communication)**: `startActivity()` triggers IPC calls to communicate with the system, which decides whether to reuse an existing activity instance or create a new one.
- **Launch Modes**: Defines how activities behave when launched. Modes such as `singleTop`, `singleTask`, and `singleInstance` determine whether activities are reused or recreated.
- **System-Managed Memory**: Activities are created via reflection and managed in system memory, which eliminates the need to define constructors in activity classes.

## Features
- Demonstrates how activities are managed in the task stack.
- Shows how the system decides whether to reuse or create activity instances.
- Provides examples of different launch modes (`standard`, `singleTop`, `singleTask`, `singleInstance`).

## Setup
1. Clone the repository:
    ```bash
    git clone https://github.com/tashafdev/ActivityTaskManagerServiceTutorial.git
    ```

2. Open the project in Android Studio.

3. Run the app on a physical device or emulator.

## Usage
- Start activities with different launch modes and observe the behavior.
- Use Logcat to track how activities are managed by the system.

## Contributing
Feel free to fork the repository and submit pull requests for enhancements or bug fixes.
