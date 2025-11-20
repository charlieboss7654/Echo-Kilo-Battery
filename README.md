[README.md](https://github.com/user-attachments/files/23661324/README.md)
# EKS Battery System

A simple, standalone battery removal system for FiveM.  
Players can remove and reinstall a vehicle's battery using **ox_target** while the hood is open.  
If the battery is removed, the vehicle will not start until it's reinstalled.


## Features

- **Remove Battery**
  - Third-eye option: **Remove Battery**
  - Only appears when:
    - You're near a vehicle
    - The **hood is open** (door index 4)
    - The battery has **not** already been removed
  - Plays a standing mechanic animation (`mini@repair`, `fixing_a_ped`)
  - Disables the engine and makes the vehicle undriveable

- **Install Battery**
  - Third-eye option: **Install Battery**
  - Only appears when:
    - Hood is open
    - Battery is currently removed
  - Uses the same mechanic animation
  - Restores vehicle power so it can start again

- **Synced Across Clients**
  - Battery state is tracked per vehicle via network ID
  - All players see the correct state (removed/installed)

- **Standalone**
  - Only dependency: **ox_target**


## Requirements

- [ox_target](https://overextended.dev/ox_target)

## Installation

1. Drop the resource folder into your `resources/` directory, for example:

   resources/
     [eks]/
       EKS_Battery/

   ## Support
   For support join the discord:
   https://discord.gg/gHvvqqNUGy
