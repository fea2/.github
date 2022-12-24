# compas_fea2

This is the `compas_fea2` organization where you can find the core library and the backend plug-ins

## Plug-in architecture

`compas_fea2` implements a plug-in architecture. The main API is defined in the
core library, while the specific backend implementations are defined in their
own plug-in library.

To use `compas_fea2` to its full capacity (i.e. to run FE simulations), you must
have at least one plug-in installed together with the main library and the
corresponding FE solver.

To set the backend plug-in (``compas_fea2_abaqus`` in this case) do as follows:

    import compas_fea2
    compas_fea2.set_backend('compas_fea2_abaqus')

Here the following plug-ins are maintained:

- ``compas_fea2_abaqus``: plug-in implementation for the Abaqus software
- ``compas_fea2_ansys``: plug-in implementation for the ANSYS software
- ``compas_fea2_opensees``: plug-in implementation for the OpenSEEs software
- ``compas_fea2_sofistik``: plug-in implementation for the Sofistik software

You can create a plug-in yourself by using the ``fea2_tpl_extension`` library.
