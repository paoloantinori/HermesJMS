HermesJMS plugin fix for autodiscovery in ActiveMQ >= 5.8 
-----------------------------------------------------------------

##### Problem

ActiveMQ, starting from version 5.8 has changed the names of some MBEANs used by Hermes plugin.

##### Fix

The code in the files

<https://github.com/paoloantinori/HermesJMS/blob/fix_activemq58/src/java/hermes/ext/activemq/ActiveMQAdmin.java>  
<https://github.com/paoloantinori/HermesJMS/blob/fix_activemq58/src/java/hermes/ext/activemq/ActiveMQAdminFactory.java>

fixes the problem.

You can build it yourself or use the `.jar` I have already built:

<https://github.com/paoloantinori/HermesJMS/blob/fix_activemq58/activemq_fix_dist/hermes-activemq.jar>

##### To install the fix:

Just copy the updated [.jar](https://github.com/paoloantinori/HermesJMS/blob/fix_activemq58/activemq_fix_dist/hermes-activemq.jar) over the old one that you can find in:

`HERMES_INSTALLATION_FOLDER/lib/ext/`

##### Reference

Based on these links:

<http://stackoverflow.com/questions/16584244/how-can-one-make-hermesjms-adn-activemqbrowser-work-withe-latest-apache-activemq/16597888#16597888>  
<http://activemq.apache.org/58-migration-guide.html>  
<http://stackoverflow.com/questions/15837853/accessing-apache-activemq-via-jmx-throws-exception>
