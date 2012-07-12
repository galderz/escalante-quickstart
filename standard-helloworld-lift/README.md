standard-helloworld-lift: Standard Hello World Lift Example
==========================================================
Author: Galder Zamarreño

What is it?
-----------

This example demonstrates that Escalante can deploy the standard, original,
helloworld example, where the war file contains all the jars required by the
Lift application, including the Scala libraries.

System requirements
-------------------

The example can be deployed using Maven from the command line or from Eclipse
using JBoss Tools or JBoss Developer Studio.

To set up Maven or JBoss Tools in Eclipse, refer to the
<a href="https://docs.jboss.org/author/display/AS71/Getting+Started+Developing+Applications+Guide"
title="Getting Started Developing Applications Guide">Getting Started Developing Applications Guide</a>.

If you're using Eclipse, or JBoss Developer Studio, a couple of extra steps
are required in order to be able to develop Scala applications. This particular
example is designed for Scala 2.9.x:

1. Install (Scala IDE)[http://scala-ide.org/docs/user/gettingstarted.html]
using the (update site for Scala 2.9.x)[http://download.scala-ide.org/releases-29/stable/site]
2. Install m2eclipse-scala via the (update site)[http://alchim31.free.fr/m2e-scala/update-site]

Remember that multiple Scala IDE instances cannot be installed under the same
Eclipse, or JBoss Developer Studio, instance, so if you want to develop in
multiple Scala versions, you'll need to maintain separate Eclipse, or JBoss
Developer Studio instaces.

Deploying the application
-------------------------

To deploy the application to Escalante using Maven, start the Escalante and type

    mvn package jboss-as:deploy

The application is deployed to <http://localhost:8080/standard-helloworld-lift>.