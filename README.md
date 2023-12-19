# Roborock-Segment-Clean
# Description
This is to provide instructions and useful tips to perform mutli-segement cleaning of your Roborock vacuum/mop in Home Assistant. This has only been tested on the S8 Pro Ultra.

# Background
The Roborock App allows for the selection of individual rooms or zones to vacuum and mop the selections. The Roborock [Home Assistant Integration](https://www.home-assistant.io/integrations/roborock/) provides for a very useful interface within Home Assistant, but as noted in the documentation, does not yet provide for individual or multiple segment or room cleaning. [Instructions](https://www.home-assistant.io/integrations/roborock/#how-can-i-clean-a-specific-room) are included in the integration page to clean individual or multiple rooms and how to identify these rooms in your logs. Identifying your rooms and the corresponding IDs is a pre-requisite to implementing individual or multi-segment cleaning.

## Requirements
1) Your room IDs as identified in [Home Assistant Integration Instructions](https://www.home-assistant.io/integrations/roborock/#how-can-i-clean-a-specific-room)
2) Input_Boolean Entities for each segment (room) -- These are toggle helpers, see [Input Boolean](https://www.home-assistant.io/integrations/input_boolean/) for more information.
3) A Group Helper to contain all of your Input Booleans from #2
4) A Script to perform segment cleaning

### Room IDs
As noted in the background, this is already explained in depth in the Roborock Integration [Instructions](https://www.home-assistant.io/integrations/roborock/#how-can-i-clean-a-specific-room)

### Input Boolean Entities
