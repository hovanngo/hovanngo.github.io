---
title: Opentrons
date: 2026-02-02 7:30:00 +/-0000
categories: [project, blog]
tags: [project]     # TAG names should always be lowercase
description: My experience as a hardware engineering co op at Opentrons Robotics
---

Collection of various engienering projets I undertook at Opentrons 

## Plate Geometry
Problem: Lots of labwares exist, with different inner well geometries. The geometry is important for a. the robot to know where the wells on a plate are relative to the deck and b. knowing where liquid height is when dispensing. 

Process: I made a novel method of mapping liquid heights to volume, utilizing a robot protocol to automatically create a look up table that is referenced when dispensing liquid. 

![IWG creator 1](/assets/img/images/IWGcreator1.jpeg "IWGcreator1")
## CMM Probe 

Problem: current calibration probe worked via capacitance, meaning it could only probe the grounded metal deck. A much more robust and practical solution would be to affix a CMM probe to the end of the pipette tip. 

Process: I created hardware firmware for a mechanical touch probe to interact with the sync line on the pipette PCB, triggering the move stop condition upon touching something. Wrote higher level drivers to utilize REPL, and wrote a series of test calibration scripts to probe previously unprobable objects at 10x speed, including labwares, modules, etc. Designed the probe mount in Solidworks, specced the drawing for manufacture in our Shenzhen office. 


![probe assembly 1](/assets/img/images/probeassembly1.jpeg "probeassembly1")

![pipette mount 1](/assets/img/images/pipettemount1.jpeg "pipettemount1")

![pipette mount 2](/assets/img/images/pipettemount1.jpeg "pipettemount2")

