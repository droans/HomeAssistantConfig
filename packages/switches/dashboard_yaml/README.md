![Switch Example 1](/images/switch_1.png)
![Switch Example 2](/images/switch_2.png)

Before using, install these frontend requirements. They can be grabbed from HACS or manually installed
* Mushroom 
* Decluttering Card
* card-mod
* fold-entity-row
* stack-in-card

You can create your own frontend instead if preferable. 
* `Mushroom` can be swapped out with appropriate replacements, but they might not be as attractive.
* `Decluttering Card` can be removed, but I find it easier to use since you can adjust the layout for all cards at once. 
* If you don't want to use `card-mod`, delete the proper sections of YAML. 
* `fold-entity-row` makes the frontend look better, but is not needed. You can manually change this yourself if you're careful.
* If you don't want to use `stack-in-card`, change the `custom:stack-in-card` types to `horizontal-stack` if `horizontal: true` is declared or `vertical-stack` if it is not. 

Next, go to your dashboard and select Edit Dashboard. Click the Menu button and select "Raw configuration editor". Scroll to the very bottom and paste everything from 'decluttering_template.yaml'.

Finally, go to the dashboard page that you want the card added. Click Add Card and select Manual Card. Paste from 'card.yaml'. Use the appropriate card template for your switches and adjust the variables to match your entities. Copy and paste the appropriate card for as many options as you need.