
debug
revision
rewrite to adapt ideas of the original code to translate MQL4 to MQL5


MQL4 and MQL5 are 2 totally different systems !! 5 is not an upgrade from 4, the company MetaTrader is maintaining
both programs, MT4 has a big community of developers and pro users.
MQL4 and MQL5 are programming languages for creating trading robots and indicators for MetaTrader 4 and 5 platforms. Here is a short explanation of their main differences with some pros and cons for each:

MQL4 and MQL5 are programming languages for creating trading robots and indicators for MetaTrader 4 and 5 platforms. Here is a short explanation of their main differences with some pros and cons for each:

MQL4 is simpler and easier to learn for beginners, while MQL5 is more advanced and closer to C++ language.

MQL4 is compatible with 32-bit operating systems, while MQL5 runs better on 64-bit operating systems.

MQL4 allows 32 buffers for one indicator, while MQL5 allows 512 buffers.

MQL4 has a limited number of built-in functions and indicators, while MQL5 has more functions and indicators, as well as access to the Market library.

MQL4 has a single-threaded strategy tester, while MQL5 has a multi-threaded and multi-currency strategy tester that is faster and more accurate.

MQL4 and MQL5 are not fully compatible with each other, so some codes written in MQL4 may not work in MQL5 and vice versa !



# convert_mql4_to_mql5

bring new life into project
deploy on https://mql4to5.herokuapp.com/

automatically convert mql4 code to mql5

Use antlr for grammatical analysis, convert mql4 code into mql5 code

Because of the incompatibility of the api layer, mql4 cannot directly generate mql5

needs to cooperate with the corresponding compatible files 

* MQL4TO5.mqh for indicator and script
* MT4Orders.mqh for EA

mql4 automatically converted to mql5 need two steps

1. Syntax conversion
   
2. api compatibility layer
