chapter 10: blockly
========================================




D:\SEANLAB2\Blockly\seanlabarduino

python  arduino_web_server.py

https://github.com/google/blockly/wiki

basic concept


D:\SEANLAB2\Blockly\node-blockly

node app.js


Disable arduino  loop with once

C:\Program Files (x86)\Arduino\hardware\arduino\avr\cores\arduino
main.cpp
	// For Once execution
	for (int i=0;i<1;i++) {
		loop();
		if (serialEventRun) serialEventRun();
	}


/*
	for (;;) {
		loop();
		if (serialEventRun) serialEventRun();
	}
*/