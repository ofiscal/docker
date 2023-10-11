# What this is

This Docker image can be used to run any code written by the Observatorio.
It is not necessary, but should always be sufficient.

See `commands.txt` in this folder for, among other things,
how to start and use it.

# PITFALL: For run-jupyter to work

The native (as opposed to docker) port must be 8888.
Running the container using one of the commands in `commands.txt` ensures this.

The 8888 requirement is a consequence of the fixed port in the `run-jupyter.sh` script.
You could opt to change that instead, but it would be more work.
However, if something else on your system also needs the 8888 port,
then changing the script is your best bet.
