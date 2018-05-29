# slack_ros
Slack ROS Bridge

## Installation
* Clone the package in your catkin workspace:

 ```git clone https://github.com/tue-robotics/slack_ros.git```

* Install required dependencies:

 ```rosdep install --from-path -y -i slack_ros```

* Build your workspace

* Additional information can be found, .e.g, [here](https://www.fullstackpython.com/blog/build-first-slack-bot-python.html)

## Setting up the slack app
* Look [here](https://www.fullstackpython.com/blog/build-first-slack-bot-python.html) again
* Create a [new app](https://api.slack.com/apps?new_app=1)
* Add a [bot user](https://api.slack.com/bot-users)
* Install the app

## Usage
* Use the 'bot user oauth access token' as the `token` parameter and run the `slack_ros_bridge` script:

 ```rosrun slack_ros slack_ros_bridge _token:=<bot user oauth access token>```

* Your Slack bot should now be available in your Slack client. Start the conversation  by entering:

  ``` /start```

* Now you can communicate with the bot:
 * Messages entered in the Slack client will be published on the `message_to_ros` topic
 * Messages received over the `message_from_ros` topic will be forwarded to the Slack conversation
 * Images send using the Slack client will be published on the `image_to_ros` topic
 * Images received over the `image_from_ros` topic will be forwarded to the Slack conversation
