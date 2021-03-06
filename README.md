# YahooFinanceD
Yahoo finance scraper written in D.

| Development Environment 	| DMD	| DUB
| ------------- 			| ------------- | -----
| Windows 10-x86     			| v2.091.1 | v1.20.1

This library obtains financial data from Yahoo based on stock's name between a begin and an end date. It has three time intervals: monthly, weely and daily. The unit test is based on scraping five stocks in a row. The implementation can be found under the [library folder](https://github.com/SelimOzel/YahooFinanceD/blob/master/lib/). I provide three examples to help new users: [json writer](https://github.com/SelimOzel/YahooFinanceD/tree/master/source/examples/json/app.d), [csv writer](https://github.com/SelimOzel/YahooFinanceD/blob/master/source/examples/csv/app.d) and a [data frame](https://github.com/SelimOzel/YahooFinanceD/tree/master/source/examples/dataframe/app.d) implementation. The dataframe allows users to access OHLC, dividend and split data on program runtime. Whereas, json and csv writers output them to external files.

**Examples:** On Windows use `dub run -a x86_mscoff yahoofinanced:example-json` to compile the json writer, `dub run -a x86_mscoff yahoofinanced:example-csv` to create two baskets of stocks and use `dub run -a x86_mscoff yahoofinanced:example-dataframe` to compile the dataframe.

**Test:** On Windows run `dub test -a x86_mscoff yahoofinanced:unittest`. 
