## Cartridge for bpmPaaS providing BPM Suite

Summary
-------
This cartridge provides the **_Red Hat JBoss BPM Suite_** for easy deployment to OpenShift based bpmPaaS.


Install bpmPaaS
---------------

To try out JBoss BPM Suite on OpenShift please follow the instructions:

If you want to use the [OpenShift create application page](https://openshift.redhat.com/app/console/application_types), enter the cartridge URI in the entry field (at the bottom left of the form:

 **https://raw.githubusercontent.com/eschabell/cartridge-bpmPaaS-6/master/metadata/manifest.yml** 

Or if you want to use the [rhc command line](https://www.openshift.com/developers/rhc-client-tools-install) type:

    rhc app create -g medium <APP NAME> https://raw.githubusercontent.com/eschabell/cartridge-bpmPaaS/master/metadata/manifest.yml

This will output the generated users and passwords for Business Central.


After installation
------------------

JBoss BPM Suite logins: 

   * u:erics   p: bpmsuite  (admin)

   * u: alan   p: bpmsuite  (analyst)

   * u: daniel p:bpmsuite  (developer)

   * u: ursla  p:bpmsuite  (user)

   * u: mary   p:bpmsuite  (manager)

   * u: larry  p:bpmsuite  (loan)

Now you can import any repository or the demo projects listed below:

1. login at business-central.

2. AUTHORING -> ADMINISTRATION -> ORGANIZATIONAL UNITS -> ADD -> 'Demos'

3. AUTHORING -> ADMINISTRATION -> REPOSITORIES -> CLONE REPOSITORY -> 'Repository Name: bpm-demos', 'Organizational Unit: Demos',
	 'Git URL: [choose-one-listed-below]

4. AUTHORING -> PROJECT AUTHORING -> inspect and run projects.

Possible demo repos:

  * https://github.com/eschabell/bpm-suite-generic-loan-repo.git
  
  * https://github.com/eschabell/bpmsuite-rewards-repo.git

  * https://github.com/eschabell/bpmsuite-customer-evaluation-repo.git

Important Note
--------------
You need the ability to setup MEDIUM gears, which is freely available if you [upgrade your account to Bronze here] (https://www.openshift.com/products/pricing). 

