# IBM Watson - Coding Tips and Tricks

This content o longer being maintained.  

## Informative and Interesting Links
- The [IBM Cloud Help](ibm.biz/ibmcloudhelp) page is an "unofficial" collection of links done by Lionel Mace.  Nice collection of places to start from.
## Annoying pop-ups asking for your credit card
If you run into the issue of an annoying pop-up window from IBM Cloud that prompts you to enter credit card information,the most likely cause is:
- You created a trial IBM Cloud account (this is probably before a corporate account subscription was initiated). Later on, a corporate IBM Cloud account is created and you were invited to work under that account. However, because the initial trial account still exists and is associated with your user id, you will continue to get the pop-up window from the IBM Cloud prompting you to enter credit card information.
- **Resolution:**
  1. Submit a IBM Cloud support ticket to delete the trial account. Make sure that you understand that **any data in that trial account will be lost!**
  1. Even though the IBM Cloud trial account is deleted, you can still log into the IBM Cloud using your id and then work under the corporate IBM Cloud account.
- **Work Around:**
  1. Log into the IBM Cloud using your account
  1. Close the pop-up message you get
  1. On top of the IBM Cloud console, click on your account and switch to the account of your organization (which is validated with subscription or paygo).  You should be able to do this, since you can access that account.

## Seeing all of your IBM Cloud organizations, spaces and applications
You are looking for a nice way to discover all of your IBM Cloud orgs, spaces, and applications.
- **Resolution:**
  1. Use the [IBM Cloud Console Tool](http://myconsole.mybluemix.net/\#/dashboard).  It is a tool deployed on the IBM Cloud that will show you all of your IBM Cloud services, spaces, applications, and organizations.
  1. If you need to get information for support, read [Getting Bluemix Information for Support and Automation](https://developer.ibm.com/dwblog/2017/getting-bluemix-information-support-automation/) for details on how to get the needed data using the [IBM Cloud CLI](https://cloud.ibm.com/docs/cli?topic=cloud-cli-ibmcloud-cli#ibmcloud-cli).  Be aware that this article is OLD, and it refers to a version of the CLI where the command was 'bluemix', it is now 'ibmcloud'.

## How do I understand IBM Cloud administration and billing?
You are unsure about how to administer your IBM Cloud account, and want to know more about how things are billed.
- **Resolution:**
  1. Read the documentation on [Building your Infrastructure](https://test.cloud.ibm.com/docs/overview?topic=overview-first-steps-it-ops#first-steps-it-ops).  It has advice on how to set up your account, monitor the usage of services by the account, and links that explain the billing procedures.
  1. You can also check out the information in [Bluemix and Watson - Getting Started Right](https://developer.ibm.com/dwblog/2017/ibm-cloud-bluemix-watson-new-customers/) for some help in understanding administration, account setup, and organization.  Be aware that this article is OLD, and some of the information in here may be out of date.
  1. Another good article on billing is [Monitoring Bluemix Usage and Spending](https://developer.ibm.com/dwblog/2017/monitoring-bluemix-usage-and-spending/), which goes over some account management basics.  Be aware that this article is OLD, and some of the information in here may be out of date.
