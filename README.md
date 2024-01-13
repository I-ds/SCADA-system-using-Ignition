# software: Ignition SCADA ver 8.1

# Export project zip and tags.json file to ignition.
# Data Logging: CSV file, MySQL db
# process description:
At the beginning, the reactor tank is empty.

We introduce 10% of the reactor volume with concentrate by operating the pump and the valve associated with the concentrate. Then, we stop the pump and close the valve.

We fill the reactor with water up to 100% of the volume by opening the water circuit valve.

We heat the mixture for 10 seconds.

We empty the reactor by operating the pump and the outlet valve until it is completely empty.

The quantity of the mixed product is added to the one already present in storage.

The outlet valve is activated according to the usage needs.

All valves are assumed to provide a flow rate of 10 liters per second.

Reactor volume: 100 liters

Product storage volume: 5000 liters

In automatic operation, the process runs in a loop until the product storage tank is completely full.

In manual operation, all valves are operated by the operator.

When the steam valve is open, the reactor temperature rises by 5° per second with an initial temperature of 20°.
# Task:
Provide process supervision with synoptics that visualize the real-time state.
Plot the temperature evolution curve of the reactor.
Plot the level curve of the reactor.
Plot the level curve of the storage.
Generate an alarm when the storage level exceeds 4000 liters.
Generate an alarm when the reactor temperature exceeds 60°C.
Propose a solution to store the dynamic process values with a 1-second sampling rate in an external file and in a database.






