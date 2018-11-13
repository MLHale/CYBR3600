# XACML Exercise

## Introduction
This exercise is to explore and practice using XACML in-class and as homework.

## Due Date
Friday November 30th (11:59 PM)

## What is Due?
You should install Wso2 Identity Management Server and play around with XACML. For each exercise below, take screenshots to demonstrate that you have completed each of the steps below. You must submit the required screenshots to Canvas for full points.

## Exercise 1 - Installing and running Wso2 Identity and Access Management server
You have several options available. I prefer using docker, but you may install the app natively.

- Visit https://wso2.com/identity-and-access-management and read about the identity access management tool.
- Install Wso2 IS

If you want to use Docker, this is really easy (beware Windows users you can only use Docker community edition with Hyper-v):
- Install docker https://www.docker.com/get-docker
- Use the pre-built Wso2 container image: https://hub.docker.com/r/isim/wso2is/
> for windows users not wishing to install Docker CE, consider installing [docker toolbox](https://docs.docker.com/toolbox/toolbox_install_windows/)
> in this case, you will also need to forward port 9443 from the container to the host. To do so, open virtual box, click settings, click network, click advanced, click port forwarding, and then forward port 9443 from guest to host, using 127.0.0.1 as the host ip.

```bash
docker pull isim/wso2is
docker run --rm --name your_container_name -p 9443:9443 isim/wso2is
```

If you don't want to use Docker or you just want to install the app natively, visit https://docs.wso2.com/display/IS530/Installation+Guide and follow the installation instructions for your preferred operating system

Once the app is running visit https://localhost:9443
The default `username/password` is `admin/admin`

Take a screenshot to show that you have the app running

## Exercise 2 - Exploring the User interface and Learning about XACML
The goal of this exercise is to actually learn how XACML works in the real world and explore the Wso2 tool.

Visit https://docs.wso2.com/display/IS530/Access+Control and read through the documentation.
Once you have a basic idea how XACML works in Wso2 visit https://docs.wso2.com/display/IS530/Identity+Server+as+an+XACML+Engine
You will be working with the policy creator and 'tryit' functionality.

Visit the PAP on your server by logging in and clicking `PAP`. Once there, click `Add Entitlement Policy` -> `Write Policy in XML`

Take a screenshot of the interface you see.

## Exercise 3 - Writing and testing policies
In this part, you will actually write some policies and test them out. Visit: https://docs.wso2.com/display/IS530/Writing+XACML2.0+Policies+in+WSO2+Identity+Server

- Go through example policy 2 here: https://docs.wso2.com/display/IS530/Writing+XACML+policies+in+WSO2+Identity+Server+-+2
- Create a new policy and copy paste the policy XML text in.
- Save the policy
- Now find it in the list of policies and click `tryit`
- Click the `create request using editor` button
- Copy paste in each request and click the `test evaluate` button to see the results of the request as determined by the `Policy Decision Point`
- Take a screenshot of the results of each request (label the screenshot Exercise 3-policy2-requestname) where requestname is `first` through `fourth`

- Go through example policy 3 here: https://docs.wso2.com/display/IS530/Writing+XACML+policies+in+WSO2+Identity+Server+-+3
- Create a new policy and copy paste the policy XML text in.
- Save the policy
- Now find it in the list of policies and click `tryit`
- Click the `create request using editor` button
- Copy paste in each request and click the `test evaluate` button to see the results of the request as determined by the `Policy Decision Point`
- Take a screenshot of the results of each request (label the screenshot Exercise 3-policy3-requestname) where requestname is `first` through `second`

## Exercise 4 - Write a request for one of the other policies (policy 4,5,6, or 7)
Write a request yourself to see what results you get. Try to get the desired behavior specified by the policy.
Copy the request text (XML) into canvas and take a screenshot of the result of evaluating your request.
