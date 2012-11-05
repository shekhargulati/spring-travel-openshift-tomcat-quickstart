tomcat6-example
===============

Sample application for Tomcat (EWS) cartridge

Create a EWS/Tomcat app on OpenShift
----------------------------

Create an account at http://openshift.redhat.com/ , don't forget to create a namespace and install client tools as well.

Create a EWS/Tomcat application

    rhc app create -a tomcat -t jbossews-1.0

Get your EWS/Tomcat running
----------------------------

Grab this quickstart codes and make it working for you!

    cd tomcat
    git remote add upstream -m master git://github.com/openshift/tomcat6-example.git
    git pull -s recursive -X theirs upstream master
    git push

That's it, you can now checkout your Tomcat at:

    http://tomcat-$yournamespace.rhcloud.com

And a sample war has been deployed already:

    http://tomcat-$yournamespace.rhcloud.com

