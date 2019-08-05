# Altcoin_API_Handler

This code allows one to get specific data from the Altcoin Trader API.

Altcoin Traders Webpage: *https://www.altcointrader.co.za/*
Altcoind Trader API:  *https://www.altcointrader.co.za/api/#/Checks/liveStats*

The Altcoin Trader API basically just allows you to get all the data for all the coins, in one shot. 
This Handler will allow you to get specific data. 

## It works as follows:

**altcoin_handler(x1,x2=None):**

The altcoin_handler method takes two arguments. The first being the coin/currency that one wants to gather info about. 
The second being the specific info one is looking for. Please note that the values are displayed in South-African Rand. 
Also note the variables are case sensitive. Meaning all the coins are written in capital letters and the second variables all start with a uppercase letter.  

for example...
```
altcoin_handler("BTC", "Price")
BTC: Price: 180501.0

altcoin_handler("XRP", "High")
XRP: High: 5.0

altcoin_handler("DOGE","Volume")
DOGE: Volume: 1838818.1
```

The second variable(x2) is not compulsory. If no second variable is given, the method will output all the data for the coin/currency in question. 

for example...

altcoin_handler("BTC")
BTC: 
        Price: 180501.00
        Sell: 182481.00
        Buy: 180350.00
        High: 183000.00
        Low: 165381.00
        Volume: 119.95
       
 >>>altcoin_handler("ETH")
 >>>ETH: 
        Price: 3678.99
        Sell: 3674.89
        Buy: 3590.00
        High: 3680.00
        Low: 3303.91
        Volume: 317.59
        
One can also give the argument of "all" to get the output of all the coin currently listed on Altcoin Trader.  

for example...
  
>>>altcoin_handler("all")
>>>BTC: 
        Price: 180030.00
        Sell: 180200.00
        Buy: 180030.00
        High: 183000.00
        Low: 165381.00
        Volume: 119.81
    
    LTC: 
        Price: 1499.00
        Sell: 1537.00
        Buy: 1487.00
        High: 1580.00
        Low: 1390.01
        Volume: 750.43
    
    NMC: 
        Price: 11.00
        Sell: 11.71
        Buy: 11.03
        High: 11.90
        Low: 10.55
        Volume: 1378.13
    
    XRP: 
        Price: 4.97
        Sell: 5.09
        Buy: 4.97
        High: 5.09
        Low: 4.94
        Volume: 174882.01
    
    ETH: 
        Price: 3678.99
        Sell: 3658.00
        Buy: 3590.00
        High: 3680.00
        Low: 3303.91
        Volume: 317.59
    
    DASH: 
        Price: 1699.00
        Sell: 1887.99
        Buy: 1637.01
        High: 1888.00
        Low: 1580.01
        Volume: 22.97
    
    ZEC: 
        Price: 1049.49
        Sell: 1049.50
        Buy: 1000.00
        High: 1093.00
        Low: 1017.50
        Volume: 7.59
    
    BCC: 
        Price: 5200.00
        Sell: 5354.80
        Buy: 5181.50
        High: 5398.00
        Low: 4966.00
        Volume: 45.53
    
    BTG: 
        Price: 283.00
        Sell: 283.39
        Buy: 282.00
        High: 283.39
        Low: 268.00
        Volume: 31.29
    
    BTCP: 
        Price: 5.63
        Sell: 5.64
        Buy: 5.63
        High: 5.70
        Low: 5.44
        Volume: 11595.84
    
    USDT: 
        Price: 15.56
        Sell: 15.45
        Buy: 15.10
        High: 15.56
        Low: 15.12
        Volume: 2378.66
    
    ADA: 
        Price: 0.8937
        Sell: 0.8939
        Buy: 0.8937
        High: 0.8939
        Low: 0.8600
        Volume: 75592.25
    
    USDT_BTC: 
        Price: 11800.00
        Sell: 13998.00
        Buy: 8501.00
        High: 11800.00
        Low: 11800.00
        Volume: 0.00
    
    NEO: 
        Price: 194.50
        Sell: 194.50
        Buy: 188.05
        High: 210.00
        Low: 182.20
        Volume: 101.04
    
    GAS: 
        Price: 31.55
        Sell: 32.70
        Buy: 31.55
        High: 32.96
        Low: 31.00
        Volume: 406.71
    
    XLM: 
        Price: 1.29
        Sell: 1.29
        Buy: 1.28
        High: 1.34
        Low: 1.26
        Volume: 18575.09
    
    TRX: 
        Price: 0.3522
        Sell: 0.3522
        Buy: 0.3510
        High: 0.3522
        Low: 0.3100
        Volume: 207290.98
    
    BSV: 
        Price: 2370.00
        Sell: 2369.50
        Buy: 2251.00
        High: 2390.00
        Low: 2200.00
        Volume: 15.70
    
    XMR: 
        Price: 1360.00
        Sell: 1469.99
        Buy: 1350.00
        High: 1553.05
        Low: 1230.00
        Volume: 15.32
    
    DOGE: 
        Price: 0.0499
        Sell: 0.0499
        Buy: 0.0472
        High: 0.0499
        Low: 0.0420
        Volume: 1838818.10
    
    BTT: 
        Price: 0.0122
        Sell: 0.0122
        Buy: 0.0122
        High: 0.0122
        Low: 0.0115
        Volume: 2311437.46
    
    XAU: 
        Price: 22887.00
        Sell: 22888.00
        Buy: 22887.00
        High: 22889.00
        Low: 22750.00
        Volume: 23.78
    
    XAG: 
        Price: 411.00
        Sell: 411.00
        Buy: 410.00
        High: 450.00
        Low: 380.00
        Volume: 713.87
    
