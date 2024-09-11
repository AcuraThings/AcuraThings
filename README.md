# Acura Kidnapping Job Script

## Overview

The `acura-kidnapping` job script is a FiveM resource for QBCore that adds a kidnapping job to your server. This job involves interacting with an NPC to start a kidnapping mission where players must wear a mask to start the job. The mission involves dealing with a kidnapped ped and 20 guards, and players will receive a reward of $5000 upon completion.

## Features

- **Start and End Missions:** Players can start and end the kidnapping mission via commands.
- **Guard Protection:** 20 guards protect the kidnapped ped.
- **Mask Requirement:** Players need to wear a mask to start the mission.
- **Reward System:** Players receive $5000 upon successful completion.

## Installation

### 1. **Download and Extract Files**

- Download the `acura-kidnapping` script.
- Extract the files into your server's `resources` folder.

### 2. **Add to Server Configuration**

Add the following line to your `server.cfg` to ensure the resource starts with your server:

```plaintext
ensure acura-kidnapping
```

### 3. **Verify Dependencies**

Ensure that you have the following dependencies installed on your server:

- `qb-core`
- `qb-target`

### 4. **File Structure**

The `acura-kidnapping` resource should have the following file structure:

```
acura-kidnapping/
│
├── client.lua
├── server.lua
├── fxmanifest.lua
│
└── ui/
    ├── ui.html
    └── ui.js
```

## File Descriptions

- **`client.lua`**: Handles the client-side logic for starting and ending the kidnapping mission, creating and managing NPCs and guards, and notifying players.
- **`server.lua`**: Manages server-side logic, including handling the start and end of the kidnapping job.
- **`fxmanifest.lua`**: The resource manifest that defines the resource and its dependencies.
- **`ui/ui.html`**: Provides the HTML interface for starting and ending the mission.
- **`ui/ui.js`**: Handles communication between the UI and the client-side script.

## Configuration

You may need to adjust the coordinates, ped models, and mask-checking logic to fit your server's needs. Edit the `client.lua` script to customize these aspects.

## Commands

- **Start Mission:** Trigger the mission with a command (e.g., `/startkidnapping`).
- **End Mission:** End the mission with a command (e.g., `/endkidnapping`).

## Troubleshooting

- **NPC/Guards Not Appearing:** Ensure that the coordinates are correctly set in `client.lua` and that the ped models are correctly referenced.
- **UI Issues:** Verify that the `ui` folder and files are correctly placed and referenced in the `fxmanifest.lua`.

## Support

For support or questions, please contact the resource author or post on the community forums.
