# zabbix_postgresql_template
Agenless remote postgresql monitoring using zabbix
===================

Postgresql Template for Zabbix (Agenless)

1. place the script "db-pgstat.pl" at zabbix-server externalscripts folder (https://www.zabbix.com/documentation/2.0/manual/config/items/itemtypes/external), make sure it has execute permission (Ubuntu - /usr/share/zabbix/externalscripts). 
2. Import the template "Template_App_PostgreSQL.xml".
3. enter you aws credentials in the template's macro section   {PG_USER_NAME},  {PG_PASSWORD}, {PG_DATABASE}
4. Attach the above template to the relevant hosts. 
5. Set the following macro on the host level - {PG_HOST_NAME} if the host name is different then the actual machine (RDS for example)

