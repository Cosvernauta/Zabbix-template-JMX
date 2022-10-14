Zabbix Templates

JMX Templates  in order to use on Zabbix.

•	Template JMX Weblogic.xml. Template so that you can monitoring different applications on Oracle Weblogic/Oracle Services Bus.

INSTRUCTIONS:

First, you must put parameters on application server:

-Djavax.management.builder.initial=weblogic.management.jmx.mbeanserver.WLSMBeanServerBuilder
-Dcom.sun.management.jmxremote -Dcom.sun.management.jmxremote.port=(Free Port)
-Dcom.sun.management.jmxremote.authenticate=false
-Dcom.sun.management.jmxremote.ssl=false
-Dcom.sun.management.jmxremote.rmi.port=(Free Port)

Then, you must configure a macro on Template with name “{$INSTANCIA}”, the value is the name server, this name is on console Oracle Weblogic. 

Last, you must attach Template JMX Weblogic and Template JMX Generic, because the Template JMX Weblogic is a complement in order to monitoring.

Enjoy it!
