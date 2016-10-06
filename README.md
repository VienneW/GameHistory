# GameHistory
The getHGameHistory is a function called by client. 
Api of client which connects to RGS, which connects to mybatis, which get access to SQL.
To show customers game history, client has to call a function and get it from SQL.


To set up the functionality, I have to import RGS(intellj idea), client API(intellj idea) and batis(eclipse).

* pay attention to the configuration of the project(on the right upper corner) set the class that I wanna run(mostly Main.class). 
* set RGS as local server.
* set appwarp_config in client API as connecting to local RGS.

modified files:
GameRoomAdaptor.java in igaming-chatapp (calling the function in BaseGameLogic.java)
BaseGameLogic.java in igaming-chatapp (calling the function in SlotgameGameCycle.java)
connection.java in RobynTest (calling the function in GameRoomAdaptor.java)
SlotgameGameCycle.java in igaming-chatapp-mybatis (calling the function in SlotgameGameCycleMapper.java)
SlotgameGameCycleMapper.java in igaming-chatapp-mybatis (mapping to sql statements in SlotgameGameCycleMapper.xml )
SlotgameGameCycleMapper.xml in igaming-chatapp-mybatis
