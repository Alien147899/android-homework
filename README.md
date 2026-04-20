# Android Homework

## 1. Task Completion

This homework was completed on a Linux system.

Completed items:

1. Android Studio was installed successfully and could be opened normally.
2. An Android Virtual Device (AVD) was created and launched successfully.
3. A simple Android app was created and run on the emulator.
4. A GitHub remote repository was created, and the project code was pushed successfully.
5. Study notes about Android architecture were prepared.

---

## 2. Simple App Result

A simple app was created in Android Studio and launched on the emulator.

The app displayed the message:

**Hello hello from avd!**

This confirms that:
- the project was created successfully,
- Gradle sync worked,
- the emulator worked,
- and the app could run correctly.

---

## 3. Android Four-Layer Architecture

Android system architecture can be understood as four main layers:

### Layer 1: Applications
This is the top layer that users directly interact with.

Examples:
- Phone
- Messages
- Camera
- Browser
- Third-party apps
- My own simple Hello app

Main idea:
- This layer contains all apps.
- Users open and use apps in this layer.
- Apps depend on lower layers to access system functions.

---

### Layer 2: Application Framework
This layer provides the main services and APIs for app development.

Important components include:
- Activity Manager
- Window Manager
- Package Manager
- Resource Manager
- Notification Manager
- Content Providers
- View System

Main idea:
- This layer acts like a bridge between apps and the lower system.
- Developers usually work with this layer when building Android apps.
- It provides reusable system services so developers do not need to build everything from scratch.

For example:
- When an app opens a new screen, it uses the Activity system.
- When an app shows a notification, it uses the Notification Manager.
- When an app accesses shared data, it may use Content Providers.

---

### Layer 3: Android Runtime and Native Libraries

This layer contains two important parts.

#### Android Runtime
Android Runtime (ART) is responsible for running Android applications.

Main idea:
- It executes app code.
- It provides core Java/Kotlin class libraries.
- It manages memory and runtime behavior.

Main idea:
- These libraries provide important functions such as graphics, database, media playback, and web rendering.
- Higher layers can call these libraries when needed.

---

### Layer 4: Linux Kernel
This is the bottom layer of Android.

Main functions:
- Device drivers
- Memory management
- Process management
- Power management
- File system support
- Security support
- Network support

Main idea:
- The Linux kernel is the foundation of the Android system.
- It directly communicates with hardware.
- It manages CPU, memory, devices, and security.

For example:
- Touchscreen driver
- Camera driver
- Audio driver
- Display driver

Without the Linux kernel, Android cannot interact with the hardware correctly.

---

## 4. My Understanding of the Four Layers

My understanding is:

- The **Applications** layer is what users can see and use directly.
- The **Application Framework** layer provides system services and APIs for developers.
- The **Android Runtime and Native Libraries** layer provides the runtime environment and important low-level functions.
- The **Linux Kernel** layer is the hardware foundation of the whole Android system.

The relationship is:

**Applications → Framework → Runtime/Libraries → Linux Kernel → Hardware**

This means the upper layer depends on the lower layer step by step.

---

## 5. Simple Text Diagram of Android Architecture

```text
Applications
    ↓
Application Framework
    ↓
Android Runtime + Native Libraries
    ↓
Linux Kernel
    ↓
Hardware


## Screenshot

<img width="1765" height="1368" alt="photo1" src="https://github.com/user-attachments/assets/c4db8fa5-8de3-402b-96e0-0143ac996d02" />

