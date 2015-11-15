Assume you have an indicator woodyFix.mq4 (available in http://mql4-connector.googlecode.com/files/MQL4Connector-2.6.38.1.zip folder examples\MT4 indicators), in order to use MQL4Connector with it, you have to
do the following:
  1. Download http://mql4-connector.googlecode.com/files/MQL4Connector-2.6.38.1.jar
  1. Open the woodyFix.mq4 file in JForex Client.
  1. Select "Translate to java".
  1. Copy the converted source and select "New indicator". Paste the copied source code. Change the source file header

FROM:
```
package jforex.converted;
import java.awt.Color;
import com.dukascopy.api.*;

public class woodyFix extends ConnectorIndicator {
```

TO (please pass the actual MQL4Connector-2.6.38.1.jar path and replace \ with /):
```
package jforex.converted;
import java.awt.Color;
import com.dukascopy.api.*;
import com.dukascopy.connector.engine.*; 
import com.dukascopy.connector.engine.Properties; 
import com.dukascopy.connector.engine.IndicatorBuffer;

@RequiresFullAccess 
@Library("C:/temp/MQL4Connector-2.6.38.1.jar")
public class woodyFix extends MQL4ConnectorIndicator {
```
> 5. Attach the indicator to a chart.