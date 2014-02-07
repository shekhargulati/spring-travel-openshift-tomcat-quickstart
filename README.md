OpenShift Tomcat 7 Spring Application 
===============

Sample application for OpenShift Tomcat 7 cartridge

Create a Tomcat 7 app on OpenShift
----------------------------

Create an account at http://openshift.redhat.com/ , don't forget to create a namespace and install client tools as well.

Create a Tomcat 7 application

    rhc app-create travelapp tomcat-7 postgresql-9.2 

Get your Spring Travel app running
----------------------------

Grab this quickstart codes and make it working for you!

    cd travelapp
    git remote add upstream -m master https://github.com/shekhargulati/spring-travel-openshift-tomcat-quickstart.git
    git pull -s recursive -X theirs upstream master
    git push

That's it, you can see the running application at:

    http://travelapp-$yournamespace.rhcloud.com
