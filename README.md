# Slack2py
A simple Slack-Python notification library, aim to send basic notification to your Slack channel by using Slack's webhook url.
### Developed By :computer:
[![N|Ranium](https://d1vxlv5w7jsf3o.cloudfront.net/wp-content/uploads/2018/10/24121043/ranium-logo-black.png)](https://ranium.in/)
##
Register or Login(if you alreday have slack account) to you workspace on [Slack]
Here's how you can grab your webhook url - https://api.slack.com/incoming-webhooks

# Install
```sh
$ pip3 install slack2py
```
# Features
- Supports multi-line notification
- notification status code (success,info,warning,danger)
- `More to come` like workspace integration, send to multiple channels etc

# Example
```python
from  slack2py import webhook

slack = webhook.setupWebhook("https://hooks.slack.com/services/{workspace_id}/{channel_id}/{token}")
                        OR
slack = webhook.setupWebhook("{webhook url}")

slack.sendNotification("Notification_title", "Error Title", "Error text", "status code options:- success,info,warning,danger")
```


   [Register]: <https://slack.com/signin>
   [Login]: <https://slack.com/signin>
