# CADET-Process

The [**CADET**](https://cadet.github.io) core simulator is a very powerful numerical engine that can simulate a large variety of physico-chemical models used in chromatography and other biochemical processes.
However, the configuration files of **CADET** can be complex and difficult to work with.
This is especially relevant when multiple unit operations are involved which is often the case for complex integrated processes.
Moreover, the structure of the configuration file may change during process optimization, for example when the order of dynamic events changes, making the direct use of **CADET** impossible without another layer of abstraction.

In this context [**CADET-Process**](https://cadet-process.readthedocs.io/en/latest/) was developed.
The package facilitates modeling processes using an object oriented model builder.
This interface layer provides convenient access to all model parameters in the system.
It automatically checks validity of the parameter values and sets reasonable default values where possible.
This simplifies the setup of **CADET** simulations and reduces the risk of ill-defined configurations files.

Importantly, **CADET-Process** enables the modelling of elaborate switching schemes and advanced chromatographic operating modes such as complex gradients, recycling systems, or multi-column systems by facilitating the definition of dynamic changes of flow sheet connectivity or any other time dependent parameters.

The package also includes tools to evaluate cyclic stationarity of processes, and routines to determine optimal fractionation times required determine common performance indicators such as yield, purity, and productivity.
Moreover, utility functions for calculating reaction equilibria and buffer capacities, as well as convenient functions for plotting simulation results are provided.

Finally, these processes can be optimized by defining an objective function (with constraints) and using one of the integrated optimization algorithms such as NSGA-3.
This can be used to determine any of the physico-chemical model parameters and to improve process performance.

---

Since CADET-Process was originally developed at FAU, it is currently being hosted [here](https://github.com/fau-advanced-separations/CADET-Process).
