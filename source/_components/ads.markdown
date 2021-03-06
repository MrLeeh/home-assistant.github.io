---
layout: page
title: "ADS"
description: "Connect Home Assistant to TwinCAT devices via the ADS interface."
date: 2016-05-25 23:39
sidebar: true
comments: false
sharing: true
footer: true
ha_category: Hub
ha_release: 0.21
ha_iot_class: "Local Push"
---

The ADS (automation device specification) describes a device-independent and
fieldbus-independent interface for communication between Beckhoff® automation
devices running TwinCAT® and other devices implementing this interface.

Configuration variables:

- **device** (*Required*): The AMS NetId that identifies the device.
- **port** (*Required*): The port that runs the AMS server on the device.
- **ip_address** (*Optional*): The IP-Address to which the Ams NetId is routed.
If None is given the first 4 bytes of the device id will be used.

```yaml
# Example configuration.yaml entry
ads:
  device: '127.0.0.1.1.1'
  port: 48898
```