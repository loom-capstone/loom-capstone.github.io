# Welcome

## Loom at Large

Loom helps researchers and developers quickly build low-cost environmental sensing systems using Arduino-compatible hardware. Designed for field-deployable sensor and actuator networks, it makes prototyping faster, deployment easier, and environmental monitoring more accessible. With Loom-V4’s simplified modular design, users can focus less on library complexity and more on collecting meaningful data in the field.

Key Features of Loom include:
- Sleep-mode via OSU OPEnS Lab custom Hypnos PCBA
- SD logging and storage
- Transmission of generated data packets using LTE or LoRa mediums
- Various supported sensors and actuators
- Microcontroller memory management

To run Loom in general, you need an Adafruit Feather m0 microcontroller, as well as the Loom library and board profile installed onto your machine. Detailed instructions for how to do this are present in the GitHub's README file

<a class="call-to-action" href="https://github.com/OPEnSLab-OSU/Loom-V4">View on GitHub</a>

### Capstone Focus

Our Capstone team focused on implementing select features to enhance Loom's existing framework. Namely, we developed a Heartbeat Dual Timer system, a Handshake system built over Loom's LoRa transmission framework, and a Location Sync system to process device locations. Additionally, we provided fixes for a backlog of long-standing bugs and improved the reliability of the Loom framework.

To run the Heartbeat system, you need a minimum of two Adafruit Feather m0 microcontrollers, as well as the Loom Library and Board Profile installed (see above on how to get Loom running). You must then open and upload either the Hypnos_Transmit.ino or Loom_Std_Transmit.ino files to the sender, found within file location examples > Heartbeat > LoRa. Then you must open and upload the generic LoRa receive.ino file, found in examples > Radios > LoRa > SinglePacket, to the receiver. Then you will be able to observe the Heartbeat system running by observing the Serial output of those processes.

## Main Module of Work: Heartbeat Dual Alarm System

The Heartbeat system was made to provide intermediary status update messages to a server during long sleep intervals between Loom sensor readings. This helps to provide a sense of surity that deployed datalogging devices out in the field are still operating as they should be, even without frequent sensor readings.

Key Features of the Heartbeat system include:
- Dual-Interval Wake Scheduling
- Transmission Medium Integration
- Visual Status Indication
- Payload Customization

<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/zPX0e9QVzN8?si=HiikpmsqIMO3XgTr" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

## Feedback

Experienced and issue? Report it on [GitHub](https://github.com/OPEnSLab-OSU/Loom-V4/issues).

## Credits

Loom has been in active development since 2022. Special thanks to all of its past [contributors](https://github.com/OPEnSLab-OSU/Loom-V4/graphs/contributors).

### Capstone Team

[Duncan Everson](https://github.com/DEusername)&emsp;
[Micah Cowell](https://github.com/cowellmi)&emsp;
[Reid Pettibone](https://github.com/ReidP-source)&emsp;
[Rory Groom](https://github.com/RoryLGroom)

## Feedback

Experienced and issue? Report it on [GitHub](https://github.com/OPEnSLab-OSU/Loom-V4/issues).

[Get Started with Loom](getting-started.md)
