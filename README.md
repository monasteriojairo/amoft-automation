# Automated MWD Oil-Fill Tool
**Team 10 – The Coogineers**  
University of Houston – MECE Capstone 2025–2026  

## Project Overview
This repository contains the control software, firmware, validation scripts,
and documentation for the Automated MWD Oil-Fill Tool.

The system consists of:

- Raspberry Pi GUI (Python)
- ClearCore motion controller (servo lift + roll)
- Arduino actuator controller (linear actuator)
- Hardwired safety chain (E-stop, brake, limits)

## Repository Structure

src/ – GUI and system control logic  
firmware/ – Arduino actuator firmware  
validation/ – Test data and analysis scripts  
docs/ – Protocol, wiring diagrams, architecture  
hardware/ – CAD exports and manufacturing drawings  

## System Architecture

Raspberry Pi → Serial → ClearCore → Servos  
Raspberry Pi → Serial → Arduino → Linear Actuator  

## Safety
The system includes:
- Hardwired emergency stop
- Power-off brake for lift axis
- Software STOP command
- Controlled descent logic
