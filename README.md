# TradeOpedia

 to run the code you have to follow the following steps:
 
 1- Make sure you have Linux operating System (you can download Virtual Machine for ease of use)
 
 2- There is a file in TradeOpedia called "venv". It is a virtual environment that can be accessed by typing the command: source venv/bin/activate
 
 3- Change the current path into Username/TradeOpedia/realtime
 
 Remove the quotations to run the commands
 
 4- type the command: "python manange.py runserver" (Make sure to download all the non existing libraries)
 
 5- type the command: "redis-server" (on different Terminal)
 
 6- type the command: "celery -A realtime worker -l info" (on different Terminal)
 
 7- type the command: "celery -A realtime beat -l info" (on different Terminal)


# Notes: 
 step 5,6,7 are for activating the real time mode for real time prices
 if redis server didn't work, try this command: "sudo service redis-server stop" then run step 5
 LSTM and KNN are deep learning models, ARIMA is a time series model and they are all used to predict the future prices
