# Actuators
Dependencies used
actuators -> to
devtools -> to restart the application for any changes added

As http actuator endpoints exposes sensitive information, so by default spring boot exposes 2 endpoint(s) beneath base path '/actuator' as they don't contain sensitive information
  /health
  /info
JMX actuators are different, as jmx actuators are inheriantly more secure than http, by default it exposes only MBeans if you are conecting from the same machine. So you can fire up jconsole from the machinge and access the application. 
    -> Open cmd prompt navigate to Java\jdk1.8.0_161\bin directory and enter jconsole
    -> select your applicationname and connect
    -> Go to MBeans tab -> org.springframework.boot -> EndPoint
    
   within JMX console, we can see the bunch of endpoints exposed.
  
