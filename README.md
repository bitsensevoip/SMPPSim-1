## SMPP Sim

### Qué es?

SMPP Sim es un simulador hecho por la empresa Selenium Software. 
En @bitsensevoip lo usamos para simular un gateway SMPP, y poder hacer tests sin la necesidad del hardware físico.

### Hoja de ruta

Ya que SMPP Sim forma parte de nuestro stack de desarrollo, queremos sumarlo como ciudadano de primera clase, por lo que forkeamos un proyecto ya existente que lo *mavenizó* y nuestra principal meta es poder ejecutarlo dentro de un container de Docker.


### Trabajo anterior y licencia

Más abajo dejamos el README original del proyecto desde donde fue *forkeado* y además dentro del archivo SMPPSim_OFFICIAL_README están descriptas las condiciones bajo las cuales Selenium Software hace publico su trabajo. 




##### Original README from haifzhan

This repo is for self learn.  I modified the origial logging to Slf4j logging which helps me for debugging:)

SMPPSim official website tutorial:
http://www.seleniumsoftware.com/user-guide.htm#quick

REQUIERD SOFTWARE:
1. java environment java 1.6.x or later.
2. maven 2.x or 3.x

QUICK START

How to run?
java -jar smppsim.jar conf/logback.xml conf/smppsim.props

How to change credentials?
All credential information is in the conf/smppsim.props

***attention***:
the smpp-lib may not be downloaded, please get the maven dependency 
in the conf/ folder and put it into your local maven repository:
/.m2/respository/smpp/smpp-lib
