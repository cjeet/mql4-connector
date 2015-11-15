## Overview ##

MQL4Connector is an open-source project that provides implementation for Metatrader 4 functions, both for strategies and indicators. MQL4Connector does not include .mq4 file conversion to java, therefore one has to convert it in JForex Client and then plug-in the library by using the @Library annotation, just as using any other include libraries:
http://www.dukascopy.com/wiki/index.php?title=Include_libraries

## Scope of application ##

What concerns running MT4 strategies/indicator in JForex client there are two logical parts:
  * Converter (carries out syntactical conversion between C-like MQL code to java JForex code).
  * Connector (implements MQL functions in JForex)
MQL4Connector replaces the latter. Meaning that if the strategy/indicator does not compile, it
still won't compile by including MQL4Connector as @Library. But if the strategy/indicator does
compile but there are problems/errors at runtime, then changes in MQL4Connector might fix them.