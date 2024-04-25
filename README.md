# droans Home Assistant Custom Config and Dashboards
---

A selection of the most useful templates, scripts, automations, and Lovelace configs I have in my HA config.

## Lovelace Mushroom Menu Card

![Example Menu](/images/menu.png)

## Multi-Press, frontend adjustable automations for your single press switches

![Switch Example 1](/images/switch_1.png)
![Switch Example 2](/images/switch_2.png)


Automations include:
* Actionable notification when garage is opened
* Automatically open the shades when you're awake, when the sun is up, and when it is not too hot outside
* Automatically open the shades when your alarm goes off
* Turn off the lights after a frontend selected delay

## Baby Dashboard and Sensors
![Example Main Baby Menu](/images/main.png)

Use the files under `dashboards/baby` and `packages/baby` along with the the `is_available` Jinja macro from `custom_templates/tools.jinja`

1. Pull a token from Babybuddy. Store it in your `secrets.yaml` as `baby_buddy_token`.
2. Change all instances of `IP_ADDRESS:PORT` to match your Baby Buddy IP Address and port.
3. Change the Entity IDs, Unique IDs, and names for all the sensors to match your needs.
4. Verify all the sensors are working properly. You may need to investigate any issues.
5. Adjust the Entity IDs in the dashboards to match your new sensors.

Sleep sensors and dashboards are not included. Those are specific to my Snoo and cameras sent via Frigate. You can set this up better for your individual scenario

All sensors which are used in the dashboard, scripts, automations, or in another sensor should have a comment above their configuration with their Entity ID to make it easier to identify and correct. Sensors without a comment are likely used in my configuration for another purpose.

Required Helpers:
* Changes:
  * input_boolean.teddy_last_diaper_solid
  * input_boolean.teddy_last_diaper_wet
  * input_datetime.teddy_last_diaper_change_time
    * Time only
  * input_select.teddy_last_diaper_color
    * Options:
      - Black
      - Brown
      - Green
      - Yellow
  * input_text.teddy_diaper_notes
* Feeds:
  * input_datetime.teddy_feeding_start
    * Time only
  * input_datetime.teddy_feeding_end
    * Time only
  * input_number.teddy_feeding_amount
  * input_select.teddy_feeding_method
    * Options:
      - Left Breast
      - Right Breast
      - Both Breasts
      - Parent Fed
      - Self Fed
  * input_select.teddy_feed_spit_up
     * Options:
       - None
       - Little
       - Some
       - A Lot
  * input_select.teddy_feeding_type
    * Options:
      - Breast Milk
      - Fortified Breast Milk
      - Formula
      - Solid Foods
  * input_text.teddy_feeding_notes
  * input_datetime.teddy_last_feed_start
    * Time only
  * input_datetime.teddy_last_feed_end
    * Time only
  * input_number.teddy_last_feed_amount
  * input_select.teddy_last_feed_spit_up
     * Options:
       - None
       - Little
       - Some
       - A Lot
  * input_select.teddy_last_feeding_method
    * Options:
      - Left Breast
      - Right Breast
      - Both Breasts
      - Parent Fed
      - Self Fed
  * input_select.teddy_last_feeding_type
    * Options:
      - Breast Milk
      - Fortified Breast Milk
      - Formula
      - Solid Foods
  * input_text.teddy_last_feed_notes
* Pumpings:
  * input_datetime.teddy_pumping_start
    * Time only
  * input_datetime.teddy_pumping_end
    * Time only
  * input_number.pumping_amount
  * input_number.teddy_last_pump_amount
  * input_datetime.teddy_last_pump_start
    * Time only
  * input_datetime.teddy_last_pump_end
    * Time only