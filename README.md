# Perfomance_generator
Performance generator, that is used with PluginSystem

## How it works
This implementation uses the PerfGen sample. It changes the code for constant value as follows: constant value is called NumberOfBytes and it shows number of bytes sent by server to client from PluginSystem. This information is read from registry.

## How to launch

1. Build solution
2. Copy the PerfGen.DLL that was built to the %systemroot%\system32 directory.
load the driver entries into the registry using the following command line: *REGEDIT PERFGEN.REG*
3. load the performance names into the registry using the command line: *LODCTR PERFGEN.INI*

After that you may find counter in the Peromance monitor - Signal - NumberOfBytes
