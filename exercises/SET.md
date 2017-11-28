# Social Engineering toolkit Exercise

## Introduction
This exercise is to explore the tools of the trade in social engineering attacks.

## Due Date
Thursday December 7th at 1:30pm.

## What is Due?
You should install the Social Engineering Toolkit (SET), create a credential harvester, capture some (of your own) user data, create a phishing attack, link the credential harvester to the attack. For each task, take screenshots of your activities.
## Ethics note
It is absolutely **not ok** to attack anyone for any reason. Using this tool for any purpose other than your own education and training is strictly prohibited by the policies of this course and University as well as local, state, and federal law. The purpose of the exercise is for you to learn about adversary tactics so that you can counter them through policy, education, and training.

## Exercise 1 - Installing and running SET
This part should be easy if you completed the XACML exercise.

Type
```docker pull mlhale/set```
either in terminal (for docker community edition users) or in docker cli (for docker toolbox users)

#### For those not using Docker
If you did not install docker before, you can do it now, or you can install SET directly:
- Install Metasploit. see: https://github.com/rapid7/metasploit-framework/wiki/Nightly-Installers
- Install the Social Engineering Toolkit. see https://github.com/trustedsec/social-engineer-toolkit

For UNIX users this translates to:
```bash
sudo apt-get install -y curl
curl https://raw.githubusercontent.com/rapid7/metasploit-omnibus/master/config/templates/metasploit-framework-wrappers/msfupdate.erb > msfinstall && \
  chmod 755 msfinstall && \
  ./msfinstall
apt-get --force-yes -y install git apache2 python-requests libapache2-mod-php \
  python-pymssql build-essential python-pexpect python-pefile python-crypto python-openssl
```
### Running SET
Once installed, you can invoke set from docker using the following command:
```bash
docker run -it -p 8888:80 mlhale/set bash
```
> Note if you are using docker toolbox, you must execute this from the docker-cli and then, using virtualbox, forward the port as you did in the XACML lesson.

In the container then type:
```bash
setoolkit
```
Follow on screen options according to the exercise you are following. Each is coded by number.

Those not using docker, may just do the latter from their local host terminal.

## Exercise 2 - Credential Harvesting
This will show you one of the most common tools used by social engineers and malicious actors to dupe you into falling prey to attack.

### Submit Screenshots
For the credential harvester show that you cloned a site by showing its web address and the interface. Type in credentials on your local host, and then submit the login button. Try several sites like facebook.com, twitter.com, and others. Take a screenshot of the password being collected in SET.

## Exercise 3 - Crafting a phishing attack
Try out the phishing attack crafting feature. It is super easy to do. You can refer to this link for more information
http://www.computerweekly.com/tutorial/Social-Engineer-Toolkit-SET-tutorial-for-penetration-testers

## Exercise 4 - Exploring Phishy links and Phishy Email
For this last part of our exploration of phishing, we are going to use some content that Dr. Robin Gandhi and I made. Visit: [https://mlhale.github.io/nebraska-gencyber/teachers/phishing/](https://mlhale.github.io/nebraska-gencyber/teachers/phishing/) and go through the url analysis and email analysis modules.

This is a good example of training and education materials that can help combat phishing attacks and spread awareness within an organization. `Gotcha hooks` are very effective for getting interested employees to care and consider the implications of their online actions.

### Submit Screenshots
For this task, take a screenshot of:
 - you inspecting each link in your browser
 - you inspecting an email header from your own inbox
