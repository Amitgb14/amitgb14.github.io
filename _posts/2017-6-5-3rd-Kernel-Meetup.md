---
layout: post
title: 3rd-Kernel-Meetup!
---


Reserved-bit organised 3rd Kernel Pune meetup on 21st May17. This meetup topic was “Overview of Power Management” by Amit Kucheria. Amit is currently working in Linaro to lead power optimization team and have great experience in power optimization.
 
The all session was interesting and we get to know how the power management system work in our latest mobile, computer and embedded devices.
 
In this session explore various subsystem related to performance and different architecture. We also get some interesting points about device battery life and performance.
 
Amit K cover lot of interesting points that we get basic understanding about how power managements works.


```
Power  ∝ Performance

If Performance want to increase then required more Power. 
If Power is down then performance also getting down.
```


Power consumption depend upon CPU performance and User requirements. But sometime user doesn’t require more performance but power consumption still remains more.
 
Example: Doesn't need more power while playing mp3 songs on your laptop or mobile device. But other component still consuming electric power. 
Disaply is one of the most power consumption component, reducing brightness is better way to save power.


Amit K also introduced [PowerTop](https://01.org/powertop). **PowerTop** is a utility tool to measure, explain and minimize computer’s electric power consumption. This tool developed by Intel and only supported linux platform.

```
$dnf install powertop -y
$powertop
```
![powertop](/images/powertop.png "powertop")

Some of the topics which Amit touched:
 
* SOC Architecture
* Power vs Performance
* Power and thermal effect
* CPUfreq, CPUIdle and other regulator
* C states and performance effect
* Cache impact with different C-states
* Memory and power management
* CPUfreq vs CPUIdle
* Dynamic Ticks
* CPU Hotplug and power management
* Runtime PM & OPP framework
* Thermal framework
* Power management stack
* Some discussion on scheduler type like CFS, EAS, SCHEDULE_DEADLINE & RT.
* Use PowerTOP tool to start working on power issues.


After the session finished we continue discussed about various topic related to power optimization, cpu, memory and other people shared there experience and asked queries.


Reference
----------
* [Power Management Session Slides](https://reserved-bit.com/wp-content/uploads/2017/06/power-management-amit-kucheria.pdf) - Amit Kucheria
* [Minutes of the meetup](http://lists.reserved-bit.com/pipermail/kernel-meetup-reserved-bit.com/2017-May/000101.html) - Pankaj Gupta


