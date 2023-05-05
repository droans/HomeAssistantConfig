Creates a 3x3 menu card for your frontend. 

![Example Menu](/images/menu.png)


Install these requirements from HACS:
* Mushroom 
* Decluttering Card
* card-mod
* stack-in-card
* layout-card

Next, copy everything from `decluttering_template.yaml` and paste it into an editor. For each item below, adjust the options to the desired choice for each menu item:
* icon: The icon for the menu item
* content: The name for the menu item
* navigation_path: The path to the menu item

You may also choose to adjust the defaults

Next, go to your dashboard and select Edit Dashboard. Click the Menu button and select "Raw configuration editor". Scroll to the very bottom and paste everything from 'decluttering_template.yaml'.

Finally, go to the dashboard page that you want the menu added. Click Add Card and select Manual Card. Paste from 'menu.yaml'. Use the appropriate card template for your switches and adjust the variables to match your entities. Copy and paste the appropriate card for as many options as you need.