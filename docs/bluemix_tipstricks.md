# Bluemix Tips and Tricks

## Annoying pop-ups asking for your credit card
If you run into the issue of an annoying pop-up window from Bluemix that prompts you to enter credit card information,the most likely cause is:
- You created a trial Bluemix account (this is probably before a corporate account subscription was initiated). Later on, a corporate Bluemix account is created and you were invited to work under that account. However, because the initial trial account still exists and is associated with your user id, you will continue to get the pop-up window from Bluemix prompting you to enter credit card information.
- **Resolution:**
  1. Submit a Bluemix support ticket to delete the trial account. Make sure that you understand that **any data in that trial account will be lost!**
  1. Even though the Bluemix trial account is deleted, you can still log into bluemix using your id and then work under the corporate Bluemix account.
- **Work Around:**
  1. Log into Bluemix using your account
  1. Close the pop-up message you get
  1. On top of the Bluemix console, click on your account and switch to the account of your organization (which is validated with subscription or paygo).  You should be able to do this, since you can access that account.

## Seeing all of your Bluemix organizations, spaces and applications
You are looking for a nice way to discover all of your Bluemix orgs, spaces, and applications.
- **Resolution:**
  1. Use the [Bluemix Console Tool](http://myconsole.mybluemix.net/\#/dashboard).  It is a tool deployed on Bluemix that will show you all of your Bluemix services, spaces, applications, and organizations.
  1. If you need to get information for support, read [Getting Bluemix Information for Support and Automation](https://developer.ibm.com/dwblog/2017/getting-bluemix-information-support-automation/) for details on how to get the needed data using the [Bluemix CLI](https://console.ng.bluemix.net/docs/cli/reference/bluemix_cli/index.html#reference).

## How do I understand Bluemix administration and billing?
You are unsure about how to administer your Bluemix account, and want to know more about how things are billed.
- **Resolution:**
  1. Read the documentation on [Managing Your Bluemix Account](https://console.ng.bluemix.net/docs/admin/account.html).  It has advice on how to set up your account, monitor the usage of services by the account, and links that explain the billing procedures.
