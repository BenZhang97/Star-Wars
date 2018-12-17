# Star-Wars
Project description 
This one Star Wars game, pick up your weapon and defeat the Dark Lordintheuniverse.In                  this game, you will drive a spaceship through the Milky Way. The spacecraft can launch               missilestohittheenemy.Ofcourse,becareful.Don'tbedestroyedbytheenemy'sspacecraft.                Theplayerscancontrolthemovementofthespacecraftthroughthefourarrowkeysandpress                the space button to launch the missile. 
 Documentation 
 
Players can control the movement of the spacecraftthroughthefourdirectionkeys,pressthe               space button to launch missiles, each hit an enemy spacecraft to gain 10 points. The game                will lose when hit by enemy spacecrafts. (If you press a direction key, the spaceship will                move in that direction all the time. When you press the key in the opposite direction, the                 spacecraft will stop moving in that direction.) 
 
Challenge and solution 
 
The main module we use is pyGame. The biggest challenge lies in the interaction of game                elements. There are three kindsofentities(Entity)inthegame.Ourspaceships,enemyships,               and missiles all have the same attributes such as position and speed. There is an interaction                between them. When our spacecraft collides with an enemy spacecraft, it crashes and loses              the game. The missile launched by the spacecraft hits the enemy spacecraft and adds 10               points. To simplify the code, the solution is to design an Entity class with move, set_speed,                display, Intersect and other methods, another challenge is collision detection, solution is the             interceptmethodintheEntityclass,usedtodeterminewhetheritcollideswithanotherEntity,               the principle is to add a radius attribute for each Entity class, when two Entity are detected                 
Collisions occur when the line distance is less than the sum of their radius.  
