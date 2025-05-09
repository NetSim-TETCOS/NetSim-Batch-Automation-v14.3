1. Open CMD window with the current directory as the location of the BatchAutoSimulation.bat file.

2. The 'Test Files' folder(s) and BatchAutoSimulation.bat should be in the same folder.

3. Run the command with 2 arguments - apppath(bin path) and license respectively:

   Open Command Prompt (cmd) in administrator mode in the current directory (Test Files).

	Method 1: USB Dongle based License 

		1. Run the below command which has 2 arguments 
			a. apppath (path to <install-dir>\bin\binx64 folder) 
			b. port@IP for license checkout
			Syntax: BatchAutoSimulation.bat <apppath> <5053@license> < nul
			Example: BatchAutoSimulation.bat "C:\Program Files\NetSim\Standard_v14_1\bin\bin_x64" 5053@192.168.0.9 < nul

		2. As soon as you hit Enter, the batch simulation starts running for the Experiments present in the Test Files folder.

	Method 2: MAC based / Cloud based License 

		1. Run the below command which has 1 argument
			a. apppath (path to <install-dir>\bin\binx64 folder) 
			Syntax: BatchAutoSimulation.bat <apppath> <License file path> < nul
		   	Example: BatchAutoSimulation.bat "C:\Program Files\NetSim\Standard_v14_2\bin\bin_x64" "C:\Program Files\NetSim\Standard_v14_2\bin" < nul

		2. As soon as you hit Enter, the batch simulation starts running for the Experiments present in the Test Files folder.

4. '< nul' is to skip the 'Terminate Batch Job(Y/N)?' message in the CMD window.

5. The simulation output files such as Metrics.xml and other files such as packet trace, event trace, animation related, logs etc can be found in the same folder containing the configuration file.

6. If you want to stop the simulation tests mid-way, close the CMD window prior to closing NetSim simulation window.

7. If you pass the wrong arguments, quit the simulation by ending the process of 'Windows Command Processor' from Task Manager.  

NOTE: Do not run the BatchAutoSimulation.bat by double-clicking. Run it only in a CMD window along with 2 arguments.

