# slack_ros
Slack ROS Bridge

## Installation
* Information can be found, .e.g, [here](https://www.fullstackpython.com/blog/build-first-slack-bot-python.html)
* Install slackclient `sudo pip install slackclient`

## Setting up the slack app
* Look [here](https://www.fullstackpython.com/blog/build-first-slack-bot-python.html) again
* Create a [new app](https://api.slack.com/apps?new_app=1)
* Add a [bot user](https://api.slack.com/bot-users)
* Install the app

## Usage
* Use the 'bot user oauth access token' as the `token` parameter and run the `slack_ros_bridge` script: `rosrun slack_ros slack_ros_bridge _token:=<bot user oauth access token>`
