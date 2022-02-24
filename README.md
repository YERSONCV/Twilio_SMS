# Twilio_SMS

## What is Twilio? 
Twilio is a customer engagement SaaS tool founded in 2008 that is used by companies like Doordash and Stripe, allowing them to make meaningful connections with their users. They put it best: 
> We’re known for democratizing channels like voice, text, chat, video, and email through APIs, making it easy for every organization to build meaningful interactions with customers on the channels they prefer.

Do you remember the transition from flip phones to iPhone, having to rewind a VCR tape to simply swiping the scroll bar on Netflix. Whether you do or not, it's clear that we have entered the digital-era and it's here to stay. **Either embrace the innovation, or lag behind** This new age has empowered indivuals to take advantage of technology to build businesses like we've never seen before. According to [Insider Intelligence](https://www.insiderintelligence.com/insights/ecommerce-industry-statistics/), amid the pandemic, US ecommerce sales will cross $1 trillion for the first time in 2022, this milestone was previously forecasted for 2024. 

There are many causes for this explosion of ecommerce including the rise in the use of mobile devices -- people are now able to buy and sell over the Internet more flexibly, quickly, and passively. In today's customer-centric world, businesses need to become more personalized and communicative through channels that are preferred by their consumers: mobile. 

Here are a few quick statistics from [Postscript's Text Messaging Statistics in 2020](https://postscript.io/blog/text-messaging-statistics): 
1. Over 77% of the entire population owns a smartphone. 
2. 68% of companies expect that mobile messaging will play a major role in consumer marketing soon. 
3. Customers are 134% more likely to respond to texts than email. 
4. The average person reads almost all of their texts, with nearly a 100% "read" rate. 

Given these stats and the growth along this horizon, there are still many opportunities for businesses to take advantage of SMS marketing and communication. It's personal, simple, outperforms other channels, and can be easily implemented with Twilio; let's get started :partying_face: 

## Users 
The users of Twilio can be segmeneted into two sections: 
1. Developers (that's us! :cowboy_hat_face:)
2. Non-technical Marketing Teams at large companies 
3. Small Businesses - ecommerce + physical services 

## Prerequisites 
- Create a [Twilio Account](https://www.twilio.com/sms) to obtain your SMS-enabled Twilio phone number. We will need our account SID and auth token. 
- Create a Ngrox Account (*optional, but non-users can only use the service for 2 hrs* 
- Download [Python 3](https://www.python.org/downloads/) 
- Download [VS Code](https://code.visualstudio.com/download) (*optional; but I will be using this text-editor throughout the tutorial*)

## Subrequisites 
For this tutorial, we are going to be leveraging virtual environments. This will allow us to isolate and organize the dependencies for this Python project. 

If you've never worked with virtual environments, don't worries! I'll give you a brief introduction to this useful tool so you can follow along with this tutorial. I reccommend checking out the [official docs](https://docs.python.org/3/tutorial/venv.html) from Python to implement this principle for future projects. 

# Welcome to Drip2Duong Coffee 
Although Drip2Duong (would be an incredibly sick name for a :coffee: brand) this is a made-up example of a small ecommerce business (user persona #3) that would use Twilio SMS in attepts to not lagging behind. 

Drip2Duong Coffee is an ecommerce brand that sells coffee beans, creamers, and accessories. They want to excelerate their sales growth in the upcoming quarter, through building a more loyal customer base. We've just been offered a free bag of beans every month to help Drip2Duong coffee use Twilio SMS to build a foundation for communicating through SMS with their customers. 

## What We are Building 
To help Drip2Duong reach their quarter goals, we are using Twilio to: 
- :outbox_tray: Send an outbound message 
- :inbox_tray: Reply to an inbound message
- :no_mobile_phones: Provide unsubscribe options 

## Setting up the Environment 
1. Create a virtual environment using `python3 -m venv coffee_venv`
- root dir: `cd Desktop` -> `mkdir drip2duong_twilio` -> `cd drip2duong_twilio` -> `python3 -m venv twilio_venv` -> `source v1_venv/bin/activate` -> cd v1twilio  -> touch send_sms_v1.py and open send_sms_v1.py
- once in vs code you want to find the right interpreter to run go to bin within the venv and type pwd to get the path 

- Create directories following this file structure: 
- Create a .env to store crednetials that will be used later on and use git ignore to make it not visible to others 
- To get into your virtual environment go to the root directory of this project, then `source drip2duong/bin/activate`
3. Once the virtual environment is started, install the dependencies via `pip3 install twilio flask python-dotenv`
4. Show how to get the VSCode terminal to run the specific environment 

1. mkdir drip2duong_twilio
2. ls
3. cd drip2duong_twilio
4. python3 -m venv twilio_venv
5. source twilio_venv/bin/activate 
6. pip3 install twilio flask python-dotenv 
7. cd twilio_venv >> cd bin >> show the dependencies that have been downloaded 
8. mkdir drip2duong
9. cd drip2duong
10. touch send_sms.py
11. open send_sms.py 

1. touch .env 
2. ls 
3. open vs code 
4. pull in console copy the account sid and auth token 
5. open back up vs code 
6. .env file 

1. import statements will not work 
2. cd .. >> cd twilio_venv/bin >> pwd 
3. Copy that path and add the root to it and tack on the python3 tag 
4. run the file and get into the VE and they should disappear 
5. 

## Sending an Outbound Message 
1. Sending a simple message 
`import os
from twilio.rest import Client` to import libraries that we will be needed 
3. what do you do with the account SID and auth token 
2. Sending a message with a photo 
- How to convert an image to a public url 
3. Scheduling a message to be sent

## Replying to an Inbound Message 
1. Twilio interface introduction 
2. Intro to post and get and running the flask app
3. Need a public url, using ngrox for that 
4. Input the forwarding address and use the web interface to ensure everything is working properly 
5. Basic text 
6. Logical statements 

## What's Next? 
Drip2Duong is now able to send messages to their customers and have opened the feedback loop by accepting inbound messages. Using everything we have learned, if we choose, we can counter offer the :coffee:/month with :coffee: + :milk_glass:/ month in exchange for the implementation of a survey option. 

You can help Drip2Duong Coffee use Twilio to send an outbound message soliciting a survey response from users over SMS. This is your chance to build upon the logic we implemented for replying to an inbound message. 

Additionally, you can pipe the responses from the text messages out of the ngrox UI and into a Google Sheet (or Airtable) so Drip2Duong can more easily access extract meaning from their customer responses. 

## References
[Twilio Developer Docs](https://www.twilio.com/docs/sms/quickstart/python)
