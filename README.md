# Commanding-And-Controlling-Drone-Using-Alexa# __Alexa voiceUI controlled Drone__

<!-- ## _Abstract_ -->

The main goal of this project is to promote and encourage autonomous aviation or unmanned flights, specifically drones, which have many potential use cases like surveillance, parcel delivery, military, search and rescue, aerial photography and mapping, agriculture, and [many more](https://www.allerin.com/blog/10-stunning-applications-of-drone-technology). 
In this project, where the drone's movement is guided using Alexa voice service, the integration of various software services/applications(AWS Lambda, WebSocket API Gateway, and more) is crucial. The below diagram depicts a brief overview of the project

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="./misc/d.png">
  <source media="(prefers-color-scheme: light)" srcset="./misc/l.png">
  <img alt="Design overview" src="./misc/l.png">
</picture>

## __Requirements__

> ### _Hardware requirements_
- Drone with [ArduPilot firmware](https://firmware.ardupilot.org/) compatible [PixHawk flight controller](https://ardupilot.org/copter/docs/common-pixhawk-overview.html)
- A computer for running a custom ground control station (GCS) software
- [SiK Telemetry Radio](https://ardupilot.org/copter/docs/common-sik-telemetry-radio.html#overview) for communication between the ground station and drone
- Amazon Echo device

> ### _Software requirements_
- Amazon Web Services [account](https://aws.amazon.com/) { Lambda, API Gateway, DynamoDB }
- DroneKit Python [API](https://dronekit.io/#air)
- Amazon developer [account](https://developer.amazon.com/) for Alexa Skill programming

## __Features__

- Voice commands
  - Takeoff
  - Change altitude
  - Fly in a specified direction for a specified distance(in meters)
  - Return to launch position
  - Know status of drone(mode, distance from home location etc..)
- Geofence 
  - A cylindrical geofence is drawn centered at the launch location
  - Commands which require the drone to fly beyond geofence radius/altitude will be discarded/rejected and not executed
  - Geofence radius and altitude are customizable
  - Radius and altitude are both measured in meters

<!-- <details>
  <summary>Potential future additions</summary>
  -> Aerial photography using a camera on the drone</br>
  -> Autonomous missions, surveys, circle and rectangle missions</br>
  -> Live footage from the camera on drone</br>
  -> LTE-powered drone to eliminate range and bandwidth issues
</details> -->

## __Setup__

1. Alexa Skill [↗](./Alexa%20Skill/)
2. AWS API Gateway WebSocket server [↗](./WebSocket%20-%20API%20Gateway/)
3. Ground Control Station application [↗](./Ground%20Control%20Station/)

## __Demo__

###### demo coming soon!
---

<details>
<summary>👇</summary>

Issues? Open an issue [here](https://github.com/prithvi2k2/Alexa-VoiceUI-Controlled-Drone/issues)</br>
Questions? Discuss [here](https://github.com/prithvi2k2/Alexa-VoiceUI-Controlled-Drone/discussions)
</details>
