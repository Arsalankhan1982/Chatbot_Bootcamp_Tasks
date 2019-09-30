# Chatbot_Bootcamp_Tasks

Task one:
Make a hotel booking chatbot with following features:

Fearures
Booking Room: 
For booking ask for name, email, number of people and type of room(vip, standard, economy) 
user should also be able to say cheap or low cost room for booking economy room

Feedback: 
For feedback ask type of feedback (complain or suggestion) subject of complain (free text) and description (free text)

Deploy this hotel booking chatbot in atleast three dialogflow supported platforms facebook, skype and google assistant.


Task Two:
Make calculation assistant with add, subtract, divide and multiply functionality
user: Hi
bot: Hi I am your calculation assistant, I will assist you in basic math problems like addition subtraction division and multiplication
user: please help me with addition
bot: I require two numbers to perform addition, please tell me your first number
user: its 4
bot: very nice you said first number is 4, what is your second number 
user: second number is 3
bot: Sum of 4 and 3 is 7

if user ask implicitly for example "what is the sum of 3 and 6" chatbot should work with it and should reply "sum of 3 and 6 is 9", 
if user ask to divide a number with zero chatbot should guide user this is an error
deploy this hotel booking chatbot in atleast three dialogflow supported platforms facebook, skype and google assistant
push all of your code with dialogflow agent export in github repo

Note: 
use firebase functions as webhook fulfilment (you may use inline editor but it is not recommended)
initialize firebase functions with typescript, it will create files in .ts format, in .ts files write whatever javascript code or typescript code.


Task Three:

Make hotel booking chatbot again from scratch using `dialogflow fulfilment nodejs` library (https://github.com/dialogflow/dialogflow-fulfillment-nodejs) instead of json request response, and also save the bookings in firestore database.


Task Four:

Make hotel booking chatbot again from scratch using `dialogflow fulfilment nodejs` library (https://github.com/dialogflow/dialogflow-fulfillment-nodejs) 

But this time use express server( https://expressjs.com/en/starter/installing.html, https://expressjs.com/en/starter/hello-world.html) instead of firebase functions deploy express server on heroku( https://devcenter.heroku.com/articles/getting-started-with-nodejs) and save bookings in mongodb database using mongoose library( https://mongoosejs.com/docs/guides.html)
use mlab( http://mlab.com) for mongodb hosting
use `mongochef studio 3t`(https://studio3t.com/) as db client


Task Five:

Weather Assistant: 
make a weather assistant chatbot with express server as webhook,
use any open weather api for getting current weather data such as open weather (https://openweathermap.org/current) 
use request module(https://www.npmjs.com/package/request) to make http request from express server to weather api
when user ask about weather ask for city name and keep remember that city name through out the context, or until I user ask question with different city name. e.g:
user: tell me about weather
bot: please mention city name to get weather detail
user: london city
bot: the temperature of London city is 22'C and humidity is 60%
user: what about rain?
bot: rain is expected in 3 hours in london city
user: what about rain in new york
bot: rain is not expected in new york city for next 24 hour  
user: tell me about wind
bot: in new york city wind speed is 7.31 km/hr and wind direction is 187.002 degrees

Task Six:

Quiz assistant:

Make an assistant which will conduct quiz(10 question) and calculate the result after asking all questions

User: hi
Bot: I'm your quiz assistant and i will conduct your general knowledge quiz, say start quiz when you are ready to start quiz

User: start quiz

Bot: what is the capital of Pakistan? Your options are karachi lahore Islamabad and blochistan

User: option 3 is correct

Bot: you said option 3, here is your next question, what is the name of Pakistani currency, your options are Dollar Rupees Yuan and darham

User: I think its option B

...
...

Bot: congratulations you answered all 10 questions, 8 out of 10 was correct, your score is 80%, do you want me to send your transcript in your email?

Make an assistant which will conduct quiz(10 question) and calculate the result after asking all questions, keep track the question in context and database combination

Note: 
use postmark as Transactional email api (https://postmarkapp.com/support/article/1002-getting-started-with-postmark)
postmark doesn't work without custom domain so buy free/paid domain from any provider like "tk domain" "godaddy" "namecheap" etc.
http://www.dot.tk/en/index.html?lang=en
https://www.namecheap.com/domains/registration/results.aspx
https://pk.godaddy.com/domains/domain-name-search

User: Yes

Bot: please let me know you email

User: malik@voiceapp.pro

Bot: your result is also sent you in your email see you next time bye.
