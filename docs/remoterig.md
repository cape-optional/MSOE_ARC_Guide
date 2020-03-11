# RemoteRig Connections, Yeasu FT-950

## Overview & Purpose

Previous to the Great Exodus of 2018, our club room was located on the third floor of the CC, on the East facing wall. This was convenient for us because all our antennas were essentially immediately above our room, making it simple and easy for the coax to be sent down through a PVC pipe into the room, and from there attached to the radios.

When then-Dean of Students Kip Kussman decided the school needed more office space, we were forced to move from this room in the CC and transfer our equipment to our current room in MLH. Thankfully we were given this new space, but it presented new problems to overcome. For instance, our antennas were not movable, and they were now a city block away, still on top of the CC. To get around this issue, we implemented a network link system, hereafter known as RemoteRig. This setup allows an operator in the MLH club room on the Yeasu FT-950 to seamlessly control the radio with all functionality, while remote-controlling an identical setup in the CC, which is where the antennas are actually connected, and where the RF is actually radiated.

## Setup in MLH

### Web Interface

This web address is the control interface for the local RemoteRig box in MLH. It should be accessible from any campus network. It offers settings for all functionality of the RemoteRig box.

**RemoteRig Box in MLH (Local):** [w9hhxedgemlh.nebula.msoe.edu](http://w9hhxedgemlh.nebula.msoe.edu)

### Hardware Connections

The setup in MLH consists of the local RemoteRig Box, the local FT-950 (MLH 950), the Club Room PC, and various other hardware and connections.

#### Yeasu FT-950

The FT-950 in MLH should be connected to 5W or higher dummy loads, on both rear antenna ports. This is for when engaging the internal antenna tuner (which is necessary to engage the internal tuner on the CC unit). The MLH 950 should NEVER be attached to a microphone, keying circuit, or RigControl/CAT cable directly! In fact, this radio should never be keyed at all, except by the internal antenna tuner function. The result could be disastrous to the finals of the radio and to the dummy loads attached. This is because the power output setting of the MLH 950 is mirrored by the CC 950, so if you want to transmit 100W out of the CC 950, the MLH 950 must be set to 100W, but the MLH 950 should never itself transmit.

All microphone connections should occur through the MLH RemoteRig box, **never** the MLH 950 front panel. All RigControl/CAT control connections must be routed through the RemoteRig box too. Remember, you are **not** trying the key the MLH 950. You are trying to key the CC 950. 

To mute the speaker of the MLH 950, a 1/4" jack adaptor has been inserted into the headphone port. The audio you want to hear (coming from the CC 950) is emitted from the audio output port of the MLH RemoteRig box.

*TL;DR: Never directly key the Yeasu FT-950 in MLH in any way, not with a microphone, not with a PC.*

#### RemoteRig Box

Useful information goes here - BHJ



## Setup in the Campus Center

### Reaching the Physical Location

The setup in the Campus Center (CC) is located in the Mezzanine level maintenance closet area. Take the double doors that face the main walkway, then turn right and open the locked door. A club advisor will provide the key. Take the hallway past the door (mind your head) until you reach an equipment cabinet on the left. This is where the CC setup is stored. In fact, it is directly above our old club room. 

### Web Interface

The following web interface links are the same address, but on different ports. The interface on explicit port 8080 is the interface for the relay box & antenna rotator unit. The interface without an explicit port number is the web interface of the RemoteRig Box in the CC.

**RemoteRig Box in CC (Remote):** [w9hhxedgecc.nebula.msoe.edu](http://w9hhxedgecc.nebula.msoe.edu)

**RotorController/Relay Box in CC:** [w9hhxedgecc.nebula.msoe.edu:8080](http://w9hhxedgecc.nebula.msoe.edu:8080)

### Hardware Connections

#### Yeasu FT-950

The two antenna ports on the rear of the CC 950 should be connected to the coaxial cables running from the roof. These are the antenna lines from the dipole and beam mounted on the roof of the CC.