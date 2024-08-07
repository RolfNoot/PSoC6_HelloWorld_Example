# PSoC6 HelloWorld Example

The PSoC6 HelloWorld Example for Visual Studio Code (CE221773_PSoC_6_MCU_Hello_World_Example)

### Say goodbye to ModusToolbox!

<em>For Windows, Linux, MacOs</em>

This example project is refactored for Visual Studio Code. Project configuration is done by the 'good old' PSoC Creator.

```
Visual Studio Code Project
│
├── .vs
│   └── (Visual Studio Code / project settings)
│
├── build
│   └── (The build output for the project: project.elf & project.hex will go here)
│
├── PSoC_Creator.cydsn
│   └── (PSoC Creator project)
│
└── source
    └── (Location of your source files: main.c, etc.)
```

## Preparation
1. Install [Visual Studio Code](https://code.visualstudio.com/download).
1. Install the OTX-Maestro extension (Sidebar > `Extensions` > search `OTX-Maestro` > `Install`).
1. All necessary tools are included in the [OTX-Maestro Tools](https://github.com/onethinx/OTX-Maestro/releases) package, which bundles the GNU ARM tools, OpenOCD, and more.
   * Download and install OTX-Maestro Tools.
1. Clone or download the project to your local machine.
   * **Hint:** To avoid build issues, keep the project directory path short by placing it close to the root directory.

## First Build and Debug!
1. Open the main project folder in VS Code.
1. Click `Clean-Reconfigure` from the status bar. This will scan the PSoC Creator folder for sources, includes, build options, etc., and include them into the project.
   * If the project wasn't initialized before, it will ask which programmer/debugger to use.
1. Click `Build` or `Build-And-Launch` to build (and launch) your project.

Enjoy!
