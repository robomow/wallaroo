# API Tester

For the API Tester, I chose to test calling the FRED API.

## What is FRED?

Short for Federal Reserve Economic Data, FRED is an online database consisting of hundreds of thousands of economic data time series from scores of national, international, public, and private sources. FRED was created and maintained by the Research Department at the Federal Reserve Bank of St. Louis.

FRED provides us with a wonderful simple use set of APIs to extract information out of its database.

## Why did I choose FRED?

We will be using the FRED API to retrieve the VIX data to help train a model in the presentation in the QuantConnect / Lean environment. 

## What is Lean?

Lean Engine is an open-source algorithmic trading engine(C# Framework) built for easy strategy research, backtesting and live trading. They integrate with common data providers (Like FRED) and brokerages so you can quickly deploy algorithmic trading strategies.

## What is QuantConnect?

QuantConnect is a company and its main product cloud-based algorithmic trading platform that uses the Lean Engine to offer its customer equities, FX, futures, options, derivatives and cryptocurrencies services. QuantConnect serves over 100,000 quants from 170+ countries, with customers including hedge funds and brokerages, as well as individuals such as engineers, mathematicians, scientists, quants, students, traders, and programmers.

## API Tester - Getting Started

The API Tester has been implemented in python as a Jupiter Notebook and Quant Algorithm in the QuantConnect platform

#The Jupiter Notebook - apitester.ipynb

 - Describes in detail what the FRED Api is and the information it will retrieve that will be used to train a model that will be eventually deployed to a real quant algorithm to improve its overall return.

 - The notebook will execute the API and show the responses it retrieved (Feel free to try to execute it yourself)


#VIXAPITester Algorithm - main.py

The VIXAPITester is a python QuantConnect Algorithm class that when executed will go back to 12/1/2020 and for each day retrieve the VIX value using the FRED API and then will plot its value
on a line graph for us to see.


## Next Step - Accessing the QuantConnect platform and executing the APITester

- Go to http://www.quantconnect.com
- Login using the credentials

user:wberger.home@gmail.com
password:Wallar00

- open the project called APITESTER - this will load up the environment
- at the top right in project section open the Jupiter notebook apitester.ipynb

  Read through it to learn all about FRED, its importance, how to test it.
- Once complete, click main.py to review how the API is embedded in the APITester python class
- Execute this by clicking on play button top middle of the screen

  This will execute the algorithm going back in tie to 12/1/2020 calling the FRED api each day to
  Obtain the VIX data

  Be patient...this can take minute or 2

- Review the results.

  You will see a line graph showing the VIX values retrieved from FRED 


That should do it.  If you made it this far, Thank you!



