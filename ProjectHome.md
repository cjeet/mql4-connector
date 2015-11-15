## Overview ##

MQL4Connector is an open-source project that provides implementation for Metatrader 4 functions,
both for strategies and indicators. MQL4Connector comes with a small GUI client for strategy/indicator conversion, which makes use of converter library which is available in [JForex public repository](http://www.dukascopy.com/client/jforexlib/publicrepo/).

What concerns running MT4 strategies/indicator in JForex client there are two logical parts:
  * Converter (carries out syntactical conversion between C-like MQL code to java JForex code).
  * Connector (implements MQL functions in JForex)
MQL4Connector replaces the latter. Meaning that if the strategy/indicator does not compile, it
still won't compile by including MQL4Connector as @Library. But if the strategy/indicator does
compile but there are problems/errors at runtime, then changes in MQL4Connector might fix them.

## Usage with MT4 indicators/strategies ##

In order to convert and use an MT4 indicator/strategy in JForex, first one has to convert the source code, which can be done with Converter Client (download http://mql4-connector.googlecode.com/files/ConverterClient%202.2.zip). Launch the application by clicking on ConverterClient.bat and then just select the source code file and if it is an indicator or a strategy. In this case we convert an indicator from examples (included in the ConverterClient 2.2.zip):

![https://lh6.googleusercontent.com/-eSvCeraFOeg/TuBhTA9RJXI/AAAAAAAAAEU/U21AXrIqXcM/s596/ConverterClient%2525200%2525201.2.png](https://lh6.googleusercontent.com/-eSvCeraFOeg/TuBhTA9RJXI/AAAAAAAAAEU/U21AXrIqXcM/s596/ConverterClient%2525200%2525201.2.png)

After a successful conversion, open the indicator in JForex client (just paste the path that the converter has already copied to clipboard):

![https://lh4.googleusercontent.com/--OLYX5ne7GA/TqVVX45XGeI/AAAAAAAAAAw/hvF4VBDIfOw/s258/ConverterClient%2525201.png](https://lh4.googleusercontent.com/--OLYX5ne7GA/TqVVX45XGeI/AAAAAAAAAAw/hvF4VBDIfOw/s258/ConverterClient%2525201.png)

Compile the indicator:

![https://lh4.googleusercontent.com/-GOxph9ddwro/TqVvd8o_99I/AAAAAAAAAB8/0VMB4ewiP5M/s570/ConverterClient%2525202.png](https://lh4.googleusercontent.com/-GOxph9ddwro/TqVvd8o_99I/AAAAAAAAAB8/0VMB4ewiP5M/s570/ConverterClient%2525202.png)

Add it to a chart:

![https://lh3.googleusercontent.com/-AoOJUYgLi1I/TqVVXemYi8I/AAAAAAAAAAo/pDuqFwDX7Js/s828/ConverterClient%2525203.png](https://lh3.googleusercontent.com/-AoOJUYgLi1I/TqVVXemYi8I/AAAAAAAAAAo/pDuqFwDX7Js/s828/ConverterClient%2525203.png)

Select "Custom indicator" and locate the compiled indicator in the file sytem (note that you have to look for .jfx file this time):

![https://lh4.googleusercontent.com/-W2C7hw-J9LU/TqVVXsRUm_I/AAAAAAAAAAs/uLvkMdwBmZE/s912/ConverterClient%2525204.png](https://lh4.googleusercontent.com/-W2C7hw-J9LU/TqVVXsRUm_I/AAAAAAAAAAs/uLvkMdwBmZE/s912/ConverterClient%2525204.png)

Allow some time for the indicator to initialize and get plotted on the chart.

![https://lh6.googleusercontent.com/-mDZ0sgMSX7E/TqVVYGnMWlI/AAAAAAAAABE/O_Xa1TUbryY/s859/ConverterClient%2525205.png](https://lh6.googleusercontent.com/-mDZ0sgMSX7E/TqVVYGnMWlI/AAAAAAAAABE/O_Xa1TUbryY/s859/ConverterClient%2525205.png)

## Usage with already converted MT4 indicators/strategies ##

See:
http://code.google.com/p/mql4-connector/wiki/Usage_with_converted
