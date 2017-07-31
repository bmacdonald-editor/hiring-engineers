# Answers to Datadog hiring-engineers assignment

### Level 0
* Set up an Ubuntu VM using Vagrant:
<image>

### Level 1
* Signed up for Datadog, and obtained local system metrics:
<image>
* Definition of the Agent: An Agent is a piece of software that runs on your host and collects data about the hardware, software, and network status. This data is transferred to Datadog, where you can view and evaluate it.
* Added custom tags to the host:
<image>
* Installed MongoDB on the virtual machine, and installed the Datadog integration for it:
<image>
* Wrote a custom Agent check that sampled a random value:
<image>

### Level 2
* Cloned the MongoDB integration dashboard, customized it, and added the `test.support.random` metric:
<image>
* Bonus question: A timeboard is a dashboard where the graphs and events are synchronized in time, so that data from all graphs can be viewed for the same time period. A screenboard contains widgets that are not synchronized, and can contain a custom layout.
Note: Graphs on a timeboard do not support snapshots. The MongoDB dashboard that I cloned is a timeboard, so I was unable to take snapshots of the custom metric from that dashboard. I was able to create a snapshot on the custom metric dashboard for the next step.
* Took a snapshot of the `test.support.random` graph, with annotation and @notification:
<image>

### Level 3
* Set up a monitor for this metric:
<image>
* Set monitor to multi-alert by host.
* Provided monitor name and message, and configured it to alert via e-mail:
<image>
* Confirmed that e-mail was received:
<image>
* Set scheduled downtime for the monitor:
<image>
Note: The downtime was specified to take place between 7:00 p.m. and 9:00 a.m. Because I created the monitor after the beginning of that period, I do not have the start of downtime notification e-mail.
