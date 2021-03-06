---
title: "Capillary Networks"
layout: post
date: 2015-09-26 12:00
tag:
- iotsi
- semantic interoperability
blog: true
star: true
---

This article is featured at the [Ericsson Research Blog](http://www.ericsson.com/research-blog/5g/evolved-capillary-networks/).

---


As the Internet of Things (IoT) becomes a reality, large numbers of very heterogeneous devices will have to be managed. How can this be done in the most efficient way?

This type of device management will expand, not only to automated software updates or error reporting of the devices, but also about how do they interact with their surroundings, with people and with other devices. That type of management will be based on the actual semantic properties of the devices. Moreover, features like energy consumption, processing power and network efficiency will be important than ever. In this context, the problem of how to manage different sensors on different locations at once becomes paramount; one single extra message per device can greatly increase network congestion.

As we wrote in our Evolved Capillary Networks blog, we initially focus on two key aspects; **Distributed Cloud** and now **Group Management**.

Short-range radio technologies can be used to connect groups of small devices to the Internet, via capillary gateways and cellular networks. But then, how do we manage the devices in these large scale sensor networks? And what’s the best way to process the data generated by these networks, so we can make use of it for real world actuation?
At the recent Mobile World Congress, we used a model railway with embedded sensors to demonstrate how we address two important aspects of IoT and sensor networks.

More than 50B devices may benefit from being connected by 2020. Many of these devices need to have minimal power consumption and low complexity, yet still be globally reachable. For example, a temperature sensor in a remote forest or in a rice field needs to run several years without changing batteries; a connected light switch needs to be very simple. These small devices can be connected using capillary gateways, which bridge the short-range radio technologies – e.g. Bluetooth, WiFi, Zigbee – used by the device to cellular networks which provide long-range connectivity. We demoed this Capillary networks concept for the first time at the Mobile World Congress 2014.

This year, we have looked at the future challenges we will face once all the different “things” in the Internet of Things are connected. Based on early insights, we focused on two aspects that we think are key questions for the connectivity of IoT and sensor networks.

To visualize these key aspects we built a model with farm land, railroads and trains carrying cargo that we used in our demo at MWC 2015. Check it out:

<iframe width="560" height="315" src="https://www.youtube.com/embed/NxtYw7ojNXg" frameborder="0" allowfullscreen></iframe>

Below, we briefly elaborate on the two questions. For those of you who want to know more about the technical details – we’ll be sharing that in two separate blog posts soon to be published.

The first question is: how can we manage the devices in these large scale sensor networks if we need to be able to get, set and execute commands on the devices. Current management protocols usually assume that there is a one-to-one mapping between the device and the manager. This could be highly inefficient if we need to address a large number of devices on which we want to modify or read some attributes. Our solution, which we demoed at MWC, is a large scale group management that could be performed by management protocols using a new concept called management proxies. Management proxies are able to broadcast commands to a group of devices as well as aggregate responses from multiple devices. This significantly reduces the number of operations we need to execute from the management interface. It also radically reduces control signaling in the network, as well as latency when executing operations on the devices.

Then we move to the second question: when we have all the IoT data that we can access, and we want to perform real world actuation based on the data generated by all the devices, what would be the way to process this data in the most efficient way? Recently, the trend has been to build large data centers where data is processed and analyzed as large data sets. This is most likely true for the future as well, when we are talking about off-line analysis of data that doesn’t require real-time control loops for control of actuation. But in order to create real-time control loops, which instantly react to data received from the sensors in a certain area, we need intelligence that is distributed on the edges of the network. In our demo, we show how virtualized software can be deployed at the edges of the network, using lightweight virtualization to create decision points that can turn simple sensor data in to multiple different actuations.

Our railway model contained over 50 sensors in total, which were used to measure what was happening in the surrounding environment. The back-end system running on the computer screen illustrated what the future connectivity provider could see on her screen when operating these networks.

The key questions and aspects of the Barcelona demo are explained a bit more in this [presentation](http://www.slideshare.net/Ericsson/capillary-networks-mwc-2015).

If you are interested in learning more about capillary networks in general, please check out this article in the Ericsson Review.

And please check back for our next posts!
