## Usage with MQL indicator ##

In order to convert and use an MQL indicator/strategy in JForex, first one has to convert the source code, which can be done with Converter Client (download http://mql4-connector.googlecode.com/files/ConverterClient%201.0.zip). Launch the application by clicking on ConverterClient.bat and then just select the source code file and if it is an indicator or a strategy. In this case we convert a strategy from examples:

![https://lh5.googleusercontent.com/-oqPWXiXW9FU/TqVuCLJ7jNI/AAAAAAAAABg/-sBtUYlp04k/s653/ConverterClient%2525200.png](https://lh5.googleusercontent.com/-oqPWXiXW9FU/TqVuCLJ7jNI/AAAAAAAAABg/-sBtUYlp04k/s653/ConverterClient%2525200.png)

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