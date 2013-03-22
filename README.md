samples to help develop jboss as 7 buildpack for cloudfoundry

* as7sample
  - http://www.mastertheboss.com/application-server/develop-java-ee-applications-with-jboss-as-7
  - you need create table by your self: create table Property (id varchar(100), value varchar(100));
* ticket-monster

 1. When you failed to build the war package of ticket-monster, check this: https://bugzilla.redhat.com/show_bug.cgi?id=87

 2. ticketmonster+database Critical error during deployment: : com.sun.faces.config.ConfigurationException: CONFIGURATION FAILED! WELD-001001 Cannot pass null expressionFactory
https://community.jboss.org/thread/221660

 3. jboss Critical error during deployment: : java.lang.OutOfMemoryError: PermGen space , try larger memory and -XX:MaxNewSize=256m -XX:MaxPermSize=256m(enlarage this two)
    (seems we don't have opportunity to set this.)
 4. deployment timeout (exceed 60s): http://www.cnblogs.com/inteliot/archive/2012/09/07/2675626.html
 5. import sample data
  
