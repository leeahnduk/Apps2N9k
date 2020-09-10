# Apps2N9k
This application helps to quickly download the Application Policies into JSON file from a Tetration Cluster and convert it into N9ks config.

## Table of contents
* [Installation](#Installation)
* [Screenshots](#screenshots)
* [How to Use](#UserGuide)
* [Files](#Files)
* [Steps to run](#Steps)
* [Feedback and Author](#Feedback)

## Installation

From sources

Download the sources from [Github](https://github.com/leeahnduk/Json2Apps.git), extract and execute the following commands

```
$ pip3 install -r requirements.txt

```

## Screenshots
![Run screenshot](https://github.com/leeahnduk/Apps2N9k/blob/master/Apps2N9k.jpg)

## UserGuide
How to use this application:
To access to the cluster you need to get the API Credentials with the following permissions
* `sensor_management` - option: SW sensor management: API to configure and monitor status of SW sensors
* `hw_sensor_management` - option: HW sensor management: API to configure and monitor status of HW sensors
* `flow_inventory_query` - option: Flow and inventory search: API to query flows and inventory items in Tetration cluster
* `user_role_scope_management` - option: Users, roles and scope management: API for root scope owners to read/add/modify/remove users, roles and scopes
* `app_policy_management` - option: 
 Applications and policy management: API to manage applications and enforce policies

Download the api_credentials.json locally and have it ready to get the information required for the setup.

A quick look for the help will list the current available options.
* To start the script, just use: `python3 app2n9k.py --url https://Cluster-IP --credential api_credentials.json `

## Files
The N9k config file will be generated as ACL_config.txt


## Steps

Step 1: Issue `$ pip3 install -r requirements.txt` to install all required packages.

Step 2: To run the apps: `python3 app2n9k.py --url https://Cluster-IP --credential api_credentials.json`

Step 3: Choose the Application you want to download and convert from the list.


## Feedback
Any feedback can send to me: Le Anh Duc (leeahnduk@yahoo.com or anhdle@cisco.com)
