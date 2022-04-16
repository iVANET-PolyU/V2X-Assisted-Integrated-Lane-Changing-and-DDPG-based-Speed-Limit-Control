
Veins - The open source vehicular network simulation framework.

simulation files: 
location: LC_Omnet\veins-veins-5.1\examples\veins
including SUMO files and omnetpp.ini
 
application files:
location: LC_Omnet\veins-veins-5.1\src\veins\modules\application\traci
RSU: MyVeinsAppRSU.cc
vehicles：MyVeinsAppCar.cc (Lane-changing control)

How to start?
1. [veins_launchd]---TraCIScenarioManagerLaunchd
D:/example_project/veins-5.1/veins-veins-5.1/sumo-launchd.py -vv -c 'D:/Program Files (x86)/Eclipse/bin/sumo.exe'
2. [manually lanch SUMO]---TraCIScenarioManager
sumo-gui -v -c llcd.sumocfg --remote-port 9999
3. [python-omnet]---TraCIScenarioManager
It is a multi-client mode, every client need to setOrder before they connected.
# sumoCmd = [self.sumoBinary, "-c", sumoConfig,"--num-clients", "2"]
# traci.start(sumoCmd, port=9999)
# traci.setOrder(1)




