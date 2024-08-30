# GCP Foundation
## Objects Relationship Maps
1. All application is installed on a foundation
2. Each application could have instance of modules
3. Before module is usable in each application, they must be activated in foundation
```mermaid
graph TD
    F(Foundation) -->|Installs| A1(Application 1)
    F -->|Installs| A2(Application 2)
    F -->|Activates| M1(Module 1)
    F -->|Activates| M2(Module 2)
    F -->|Activates| M3(Module 3)

    A1 -->|Has Instance of| M1
    A1 -->|Has Instance of| M2
    A2 -->|Has Instance of| M2
    A2 -->|Has Instance of| M3
```

## GCP Foundation Introduction
## Usage
### Preparation

### Initialization of modules
Initialization of the module to be used in cosmos
`make init-module module_uri=<package_name>@<version>/<module_name>"`

### Activation of modules
Activation of the module to be used in foundation
`make init-module module_uri=<package_name>@<version>/<module_name>"`
