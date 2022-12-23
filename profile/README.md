# compas_fea2

This is the `compas_fea2` organization where you can find the core library and the backend plug-ins

## Plug-in architecture

`compas_fea2` implements a plug-in architecture. The main API is defined in the
core library, while the specific backend implementations are defined in their 
own plug-in library.

To use `compas_fea2` to its full capacity (i.e. to run FE simulations), you must
have at least one plug-in installed together with the main library and the
corresponding FE solver.
