---
layout: default
title: Heroku ClearDB MySQL Server Setup Guide
---
# Heroku ClearDB MySQL Server Setup Guide

This guide assumes that you have already set up a Heroku account and walks you through the steps necessary for adding a MySQL Server to your account.

- Log in to your Heroku account
- On your "Dashboard" click on the plus sign on top-right of the screen to create a new app
- Once asked for an app name, give it a unique name or leave the field empty so that Heroku generates one for you
- Go to the "Resources" tab and click "Get more addons..."
- In the following page, scroll down and choose "ClearDB MySQL Database"
- Scroll down, select the app you just created in the drop-down menu and press "Add Ignite for Free"
- Heroku may ask you to log in again or to add your credit card information. Please do so and then come back to this page by going back to your "Dashboard", selecting your app and then selecting "Get more addons..."
- Once this is done, and your database is added, go back to your project in the Dashboard and under the settings tab click "Reveal Config Vars"
- Select the entire field starting with "mysql://" and copy and paste the content in a text file. What you have got is a connection string that we need to dissect and feed into MySQLWorkbench. You should have received a string like this: `mysql://b251d87417a039:c03d64f0@us-cdbr-iron-east-01.cleardb.net/heroku_1f5e4e668bec9aa?reconnect=true`

Let's break it down:

| __Text__                           |  __Content__   |
|------------------------------------|:--------------:|
| `mysql://`                         | -              |
| `b251d87417a03`                    | Username       |
| `:`                                | -              |
| `c03d64f0`                         | Password       |
| `@`                                | -              |
| `us-cdbr-iron-east-01.cleardb.net` | Hostname       |
| `/`                                | -              |
| `heroku_1f5e4e668bec9aa`           | Default Schema |
| `?reconnect=true`                  | -              |

- Now go to MySQLWorkbench's Home window and click the plus sign to create a new connection
- Populate the form with the data from the connection string that you have dissected like above
- Test the connection
- Press OK to close the edit window and now connect to the connection by clicking on the connection in the home window
