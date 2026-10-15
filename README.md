# ATmega16u2 Custom Gamepad Hardware Design

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=flat-square)](https://opensource.org/licenses/MIT)
[![KiCad](https://img.shields.io/badge/KiCad-FFFFFF?style=flat-square&logo=kicad&logoColor=blue)](https://www.kicad.org/)

A custom-designed printed circuit board (PCB) for a gamepad based on the ATmega16u2 microcontroller. This repository includes the full schematic capture, layout, and manufacturing-ready fabrication files.

##  Table of Contents
- [About the Project](#about-the-project)
- [Tech Stack](#tech-stack)
- [Getting Started](#getting-started)
- [Repository Structure](#repository-structure)

##  About the Project

This project contains the complete hardware design files for a custom USB gamepad. Utilizing the ATmega16u2, the board is designed to handle button inputs and communicate with a host PC or console as a standard USB Human Interface Device (HID). 

### Tech Stack
*   **EDA Software:** KiCad (for schematic capture and PCB layout)
*   **Hardware Target:** ATmega16u2 Microcontroller

##  Getting Started

Follow these instructions to view or modify the hardware design files locally.

### Prerequisites

*   [KiCad EDA](https://www.kicad.org/download/) to open the core project files.
*   A PDF viewer to read the exported schematics.
*   A Gerber viewer (if you only want to inspect the manufacturing layers).

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/MohamedHassanExp/game-pad.git
2. Navigate to the project directory
   ```bash
   cd game-pad--main
3. Open `Hardware/game pad atmega 16u2 based.kicad_pro` project file using KiCad.

## Repository Structure

The repository is organized to separate the editable design files from the static manufacturing outputs:

*   **Design Files:**
     The Hardware/ directory contains the core KiCad project files, including the schematic (game pad atmega 16u2 based.kicad_sch), the physical layout (game pad atmega 16u2 based.kicad_pcb), and a PDF export of the design (game pad atmega 16u2 based.pdf).
*    **Board Renders:**
      High-resolution 3D renders of the physical layout are available as game pad atmega 16u2 based-front.png and game pad atmega 16u2 based-back.png.  
*    **Manufacturing Files (Hardware/Manufacturing/):** 
      This directory contains everything a fabrication house like JLCPCB or PCBWay needs to manufacture and assemble the board:
      * **game pad atmega 16u2 based-gerber.rar:** The compressed Gerber layers and drill files for PCB fabrication.
      * **game pad atmega 16u2 based-BOM.csv:** The complete Bill of Materials for component sourcing and assembly.
      * **game pad atmega 16u2 based-position.csv:** The centroid/pick-and-place data for automated SMD assembly.
