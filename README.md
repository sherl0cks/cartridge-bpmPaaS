## Cartridge for bpmPaaS providing BPM Suite

This cartridge provides the **_Red Hat JBoss BPM Suite_** for easy deployment to OpenShift based bpmPaaS.


Install with one click in xPaaS (bpmPaaS)
-----------------------------------------
After clicking button, ensure `Gear` size is set to `medium`:

[![Click to install OpenShift](http://launch-shifter.rhcloud.com/launch/light/Click to  install.svg)](https://openshift.redhat.com/app/console/application_type/custom?&cartridges[]=https://raw.githubusercontent.com/jbossdemocentral/cartridge-bpmPaaS/master/metadata/manifest.yml&name=bpmpaas&gear_profile=medium&initial_git_url=)

Once installed you can use the JBoss BPM Suite login: 

   * u:erics   p: bpmsuite  (admin)

   * u: alan   p: bpmsuite  (analyst)

   * u: daniel p: bpmsuite (developer)

   * u: ursla  p: bpmsuite (user)

   * u: mary   p: bpmsuite (manager)

Important Note
--------------
You need the ability to setup MEDIUM gears, which is freely available if you [upgrade your account to Bronze here](https://www.openshift.com/products/pricing). 


Manual setup on OpenShift
-------------------------
Or if you want to use the [rhc command line](https://www.openshift.com/developers/rhc-client-tools-install) type:

    rhc app create -g medium <APP NAME> https://raw.githubusercontent.com/jbossdemocentral/cartridge-bpmPaaS/master/metadata/manifest.yml

This will output the generated users and passwords for Business Central.

Now you can import any repository or the demo projects listed below:

1. login at business-central.

2. AUTHORING -> ADMINISTRATION -> ORGANIZATIONAL UNITS -> ADD -> 'Demos'

3. AUTHORING -> ADMINISTRATION -> REPOSITORIES -> CLONE REPOSITORY -> 'Repository Name: bpm-demos', 'Organizational Unit: Demos',
	 'Git URL: [choose-one-listed-below]

4. AUTHORING -> PROJECT AUTHORING -> inspect and run projects.

Possible demo repos:

  * https://github.com/jbossdemocentral/bpm-suite-generic-loan-repo.git
  
  * https://github.com/jbossdemocentral/bpmsuite-rewards-repo.git

  * https://github.com/jbossdemocentral/bpmsuite-customer-evaluation-repo.git

