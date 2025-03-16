# PanAIO quicktask documentation

### Quicktask Structure

<pre><code>
 https://www.panaio.com/quicktask?link={productLink}
 
</code></pre>

 
### Examples of quicktask
<pre>https://www.panaio.com/quicktask?link=https://www.asos.com/new-balance/new-balance-530-trainers-in-off-white-and-beige/prd/204936689 </pre>

### Country
You can optionally specify the country in the quicktask if you want to force a country on a task, please note that this is not a suggested approach since users usually set their country in the bot, the country is not mandatory, you can add it with this format country={country} with the country being lowercase

 ### Additional parameters
We also support other optional additional parameters such as:
 * method, used to set payment method of the task, the value should match the payment method name in the PanAIO GUI
 * mode, used to set mode of the task, the value should match the mode in the PanAIO GUI
 * quantity, used to sent quantity of the item
 * priceLimit, used only on amazon to specify the maximum of an item, if the item price should be less than 100€ for example priceLimit must be set to 100
 * details, used only on amazon to specify an offerid this must be used with Fast mode, usage is details={offerid}

Other parameters might still be supported even if undocumented, please open a ticket in our discord support server if you have some specific questions https://discord.gg/AvgQ2EMW
