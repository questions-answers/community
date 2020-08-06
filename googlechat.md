---
layout: default
---

# Google Chat integration

This guide describes how to send notifications about new questions to Google Chat room.
In order to setup integration with Google Chat, you need to:

#### Define an incoming webhook in Google Chat's room

From the chat room menu select _Manage Webhooks_

![image](https://user-images.githubusercontent.com/731629/89202017-a35e9080-d5b2-11ea-985b-c3d66bd1ea78.png)

Then, you should see a form used to create new webhook (you'll need to click _Add another_ if you already have some webhooks defined). Type webhook's name and press save 

![image](https://user-images.githubusercontent.com/731629/89202322-0ea86280-d5b3-11ea-8197-397294cdd24f.png)


Created webhook should appear on a list of all webhooks defined for this room. Copy link of this webhook, we'll need it in next step

![image](https://user-images.githubusercontent.com/731629/89202430-37305c80-d5b3-11ea-90ef-249cd152817b.png)


#### Connect Confluence space to Google Chat room by using previously created webhook

Now with webhook created, we can continue to the next step which is Confluence space configuration. 
Open _Questions and Answers for Confluence_ space settings of space you'd want to connect. Press _Connect to Google Chat_ button

![image](https://user-images.githubusercontent.com/731629/89202918-fe44b780-d5b3-11ea-88fa-237e9c71f656.png)

Paste webhook and click _Connect_

![image](https://user-images.githubusercontent.com/731629/89203038-2cc29280-d5b4-11ea-88cd-94f300470817.png)

And that's all! You should now get notification about new questions to your Google Chat room, similar to one below:

![image](https://user-images.githubusercontent.com/731629/89203124-511e6f00-d5b4-11ea-85b7-96ef9a33ce22.png)

### Limitations 

All organizational units in your domain need to have bots enabled, otherwise Google Chat notifications won't work. 
[Read more](https://developers.google.com/hangouts/chat/how-tos/webhooks#limitations)

### Troubleshooting

##### Cannot create webhook
Users need to have _Allow users to add and use incoming webhooks_ permission in order to be able to create webhooks. 
Read more about it in [Turn on incoming webhooks in Chat](https://support.google.com/a/answer/7651360) section.


### References

* [Using incoming webhooks in Google Chat](https://developers.google.com/hangouts/chat/how-tos/webhooks)
* [Allowing Google Chat users to use bots](https://support.google.com/a/answer/7651360)

