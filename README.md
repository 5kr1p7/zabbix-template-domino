Zabbix template for monitoring IBM Lotus Domino
======================================

This is a template for [Zabbix monitoring system](http://www.zabbix.com/ "Zabbix website").

How to configure Lotus Domino
---------------------------------------------
1. [Install and setup windows SNMP service](https://support.powerdnn.com/KB/a764/how-to-install-snmp-and-configure-the-community-string.aspx) (community and allowed clients)
- Launch lnsnmp.exe -Sc from Domino directory for install Lotus SNMP service
- Restart SNMP services:
 <pre>
net stop snmp
net stop lsnmp
net start snmp
net start lsnmp
 </pre>

- In Domino Console load tasks what are you need:<br />
  ``load quryset`` for SNMP queries<br />
  ``load intrcpt`` for SNMP traps<br />
  ``load collect`` for statistics threshold traps
