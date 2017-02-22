# Google Analytics Measurement Connector

The Google Analytics connector enables you to send measurement events to Google Analytics from your Microflows.

 ![Google Analytics toolbox][1]
 
There are 3 actions you can use:

* Track PageView - Can be used to register a pageview by the user, instead of using a widget on your page.
* Track Event - Track any event in your microflow.
* Track Exception - Track exceptions in your microflows.

More info on using Google Analytics measurements api can be found here: [Measurement Protocol Overview][2]

 ![Google Analytics track event example][3]

## Development

The sourcecode for these Connectors can be found on Github: [Mendix MxUtils][7]

All java jar dependencies are managed using an ivy file. You can download all
dependencies by running runivy.cmd. This will save all jars in the userlib folder. There are two different
scripts to run ivy:
* runivy.cmd - downloads all dependencies required for running and testing the project
* runivy-export.cmd - downloads only the dependencies required for distributing the connector mpk.

Before you start to develop the connector you need to run runivy.cmd. After you validate everything works, run runivy-export.cmd.
This will delete all jars in the userlib folder and only download the jars required for creating the connector mpk.

 [1]: docs/images/google_analytics_toolbox.png
 [2]: https://developers.google.com/analytics/devguides/collection/protocol/v1/
 [3]: docs/images/ga_track_event_example.png

