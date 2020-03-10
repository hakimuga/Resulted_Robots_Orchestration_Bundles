# ROBOT SYSTEM ORCHESTRATION

**Five bundles are now available for deployment**
*  1- Import the Maven files located in  Orchestrator_Web_Interface directory 
*  2- Locate single-framework-example and lunch debug.bndrun
*  3- Click run OSGi
*  4- Go to http://localhost:8080/main
*  5- Type the ip address and port (IP:10.8.0.50 PORT:8080)
*  6- If the page returned =>" Host : 10.8.0.50 is reachable "  Then the server is available and robots will start 




# BIP_To_Java

> This is a first prototype for the resulting BIP to Java Mapping 



**Bundles for remote execution**
*  1- Import the Maven files located in Robot Remote Bundles in Eclipse Photon Version
*  2- In the entity application folder, for example, door-app, open the debug.bndrun and start the OSGi.
*  3- Check the relevant file (the business implementation), for example, door-impl, by typing lb.
*  4- Start the door-impl, orch-impl and robot-impl by typing the command door, orch, and robot, respectively.
>    `During the execution you will see that the orchestrator asks the robot to move to the unload location at the first step and then it will ask the robot to move to the docking.`




**BIP To Java Plug-in**

**Follow these instructions to install the BIP To Java Plug-in (I successfully deployed it on Linux-64 bits):**

*  1- Download and Uncompress one the Eclipse version located in : 
>          Linux 64-bits :http://download.polarsys.org/3p/PolarSysIDE/0.8/org.polarsys.ide.0.8-incubation-linux.gtk.x86_64.tar.gz
>          Windows 64-bits : http://download.polarsys.org/3p/PolarSysIDE/0.8/org.polarsys.ide.0.8-incubation-win32.win32.x86_64.zip
>          Windows 32-bits : http://download.polarsys.org/3p/PolarSysIDE/0.8/org.polarsys.ide.0.8-incubation-win32.win32.x86.zip




* 2- Download and Uncompress the developed Plugin `org.verimag.feature.bip.update.zip` in a specific directory         
* 3- Go To Help | Install New software 
* 4- Add the location of the Archive file ( from the directory where the Plugin was uncompressed) : The repo should look like :
>  `BIP - file:/home/Brain-IoT/Poly/Eclipse/org.verimag.feature.bip.update/` 

* 5- Select org.verimag.feature.bip  and click Next
* 6- Select BIP feature and click Next
* 7- Accept the terms of license and click Finish (In case of exception click OK)
* 8- Eclipse will restart
* 9- Import the BipToJavaCase10 (from the directory where the archive was uncompressed). (Some Eclipse versions require to change the java version to support annotations)
* 10- Try to remove "Atom package" and make some update on the BIP model -> The "Atom package" will be automatically created

