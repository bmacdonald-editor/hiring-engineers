# Answers to Datadog hiring-engineers assignment

### Level 0
* Set up an Ubuntu VM using Vagrant:
![Ubuntu box](https://github.com/bmacdonald-editor/hiring-engineers/blob/master/Ubuntu%20box.jpg)

### Level 1
* Signed up for Datadog, and obtained local system metrics:
![Local system metrics](https://github.com/bmacdonald-editor/hiring-engineers/blob/master/Local%20system%20metrics.jpg)

* Definition of the Agent: An Agent is a piece of software that runs on your host and collects data about the hardware, software, and network status. This data is transferred to Datadog, where you can view and evaluate it.

* Added custom tags to the host:
![Host map with custom tags](https://github.com/bmacdonald-editor/hiring-engineers/blob/master/Host%20Map%20with%20custom%20tags.jpg)

* Installed MongoDB on the virtual machine, and installed the Datadog integration for it:
![MongoDB integration](https://github.com/bmacdonald-editor/hiring-engineers/blob/master/MongoDB%20integration.jpg)

* Wrote a custom Agent check that sampled a random value:
![Custom random metric](https://github.com/bmacdonald-editor/hiring-engineers/blob/master/Custom%20random%20metric.jpg)

### Level 2
* Cloned the MongoDB integration dashboard, customized it, and added the `test.support.random` metric:
![Custom dashboard](https://github.com/bmacdonald-editor/hiring-engineers/blob/master/Custom%20dashboard.jpg)

* Bonus question: A timeboard is a dashboard where the graphs and events are synchronized in time, so that data from all graphs can be viewed for the same time period. A screenboard contains widgets that are not synchronized, and can contain a custom layout.

**Note:** Graphs on a timeboard do not support snapshots. The MongoDB dashboard that I cloned is a timeboard, so I was unable to take snapshots of the custom metric from that dashboard. I was able to create a snapshot on the custom metric dashboard for the next step.

* Took a snapshot of the `test.support.random` graph, with annotation and @notification:
![Snapshot with annotation](https://github.com/bmacdonald-editor/hiring-engineers/blob/master/Test.support.random%20with%20annotation.jpg)

### Level 3
* Set up a monitor for this metric:
![Monitor creation](https://github.com/bmacdonald-editor/hiring-engineers/blob/master/Monitor%20creation.jpg)

* Set monitor to multi-alert by host.

* Provided monitor name and message, and configured it to alert via e-mail:
![Alert notification](https://github.com/bmacdonald-editor/hiring-engineers/blob/master/Test.support.random%20alert%20notification.jpg)

* Confirmed that e-mail was received:
![Alert e-mail] (https://github.com/bmacdonald-editor/hiring-engineers/blob/master/Alert%20e-mail.jpg)

* Set scheduled downtime for the monitor:
![Alert downtime](https://github.com/bmacdonald-editor/hiring-engineers/blob/master/Schedule%20alert%20downtime.jpg)

**Note:** The downtime was specified to take place between 7:00 p.m. and 9:00 a.m. Because I created the monitor after the beginning of that period, I do not have the start of downtime notification e-mail.
