---
title : "Teleoperation issues"
description: "VR teleoperation application FAQ"
lead: "Frequently asked questions on VR teleoperation application"
date: 2023-07-26T08:44:51+02:00
lastmod: 2023-07-26T08:44:51+02:00
draft: false
images: []
type: docs
menu:
  help:
    parent: "FAQ"
toc: true
weight: 230
---

## Problem with the cameras or sound

### With teleoperation application

During teleoperation, the cameras and sound are managed by the webrtc service.  
This service is automatically launched when you start Reachy 2 computer. 

> If you have switched between the Python SDK and the teleoperation application without robot rebooting, first make sure:
>- that any running client to the sdk has been disconnected
>- that the speaker has been plugged back
>- that the webrtc services has been restarted

Check all logs of the service with:

```bash
journalctl -b -u webrtc
```
