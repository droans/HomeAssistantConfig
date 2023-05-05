Frontend adjustable switch automations that enable different actions to be taken for different number of button presses. Made to work with switches that do not report multiple presses on their own.

Designed for the [Ikea Tradfi 5 button remote (E1524/E1810)](https://www.zigbee2mqtt.io/devices/E1524_E1810.html) and the [Philips Hue Dimmer Switch (324131092621)](https://www.zigbee2mqtt.io/devices/324131092621.html). These will likely work with any other switch but will require the user to adjust multiple files and perform the necessary debugging on their own.

All files here are designed to work together. You may swap them out for your own preferred options, but I will not provide assistance. 

Add the files in this order:
* All files under `options`
* `multipress_automation_helper_sensors.yaml`
* `multipress_action_inputs_hue.yaml` and/or `multipress_action_inputs_ikea.yaml`
* `multipress_sensors.yaml`
* `multipress_actions.yaml`

To create the frontend adjustment card:
* `multipress_frontend_select.yaml`
* `dashboard_yaml/decluttering_template.yaml` (**READ THE README FILE FIRST**)
* `dashboard_yaml/card.yaml` (**READ THE README FILE FIRST**)
