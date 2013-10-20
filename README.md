Zabbix template for IBM Lotus Domino
======================================

This is a template for [Zabbix monitoring system](http://www.zabbix.com/ "Zabbix website").

How to configure Lotus Domino (Windows)
---------------------------------------------
1. [Install and setup windows SNMP service](https://support.powerdnn.com/KB/a764/how-to-install-snmp-and-configure-the-community-string.aspx) (community and allowed clients)
2. Launch ``lnsnmp.exe -Sc`` from Domino directory for install Lotus SNMP service
3. Restart SNMP services:
 <pre>
net stop snmp
net stop lsnmp
net start snmp
net start lsnmp
 </pre>
4. In Domino Console load tasks what are you need:<br />
  ``load quryset`` for SNMP queries<br />
  ``load intrcpt`` for SNMP traps<br />
  ``load collect`` for statistics threshold traps

How to configure Lotus Domino (Linux)
---------------------------------------------
TODO
Instal and configure template
---------------------------------------------
TODO
