messy cause it's a work in progress 🙄

//brainstorming
- simulation using agent-based modelling
- 3 main sets of agents (15 airplanes, ATC tower, runway)
- database: excel sheet with scheduled arrival/departure times, destination and initial location for each aircraft
- role of ATC: send status of runway to aircrafts - communicates with aircrafts on availability of runway
- runway status is stored in variable runwayStatus
- each aircraft will contain 1 sensor - warns when 1 aircraft is too close (around 200m)to another


## issues/ constraints
1. it's simulated for a day, but since it's built using the road from the road traffic library (RTL), the simulation is only allowed to run for an hour
2. simulation doesn't work when scale is in km - probably cause of the RTL
3. using PLE version of AnyLogic- no option to connect path to moveTo- have to resort to using road from RTL
4. can't customise initial location and schedule of each airplane if in agent population - have to create 15 different agents for each airplanes (???? is it PLE? weird.)


## TO DO
1. set variable for runway status
2. set variable for aircraft status
3. maybe: add lights near ATC to inform about status of runway ^

check: 
1. link database to simulation- what part of the simulation? which agent?
2. should there be any new connections?


^ lights messages:
- red: runway occupied
- yellow: can taxi, prepare to move towards runway
- green: runway available- prepare for takeoff and takeoff/arrival
