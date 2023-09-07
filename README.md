# PanAIO quicktask documentation

### Quicktask Structure

<pre><code>
 https://www.panaio.com/quicktask?site=&lt;site&gt;&link=&lt;productLink&gt;
 
</code></pre>

 
****site = Kith**** <br>
****productLink = https://eu.kith.com/collections/mens-footwear/products/jbct4838-011**** <br>


### Examples of quickTask
<pre> https://www.panaio.com/quicktask?site=Kith&link=https%3A%2F%2Feu.kith.com%2Fcollections%2Fmens-footwear%2Fproducts%2Fjbct4838-011 </pre>

#
### Site
***The brackets next to the sites indicate that the parameters specified can be entered instead of the productLink***

 **Values to insert in the variable site**
  * About You (link, pid)
  * Adidas (link, pid)
  * Airness (link, pid)
  * Amazon (link, pid)
  * Asos (link, pid)
  * Awlab (link, pid)
  * Boozt (link, pid)
  * Cisalfa (link)
  * Disney (link, pid)
  * End Clothing (link, pid)
  * Fnac (link, pid)
  * Footpatrol (link, pid, sizepid)
  * Here Store (link, pid)
  * H&M (link, pid)
  * JDSports (link, pid, sizepid)
  * Kith (link, pid)
  * LVR (link, pid)
  * Micromania (link, pid)
  * Myntra (link, pid)
  * NBSklep (link, pid)
  * New Balance (link, pid)
  * QueueIT (link)
  * Rinascente (link, pid)
  * Shopify (link)
  * Size (link, pid, sizepid)
  * Snipes (link, pid)
  * Solebox (link, pid)
  * TheHipStore (link, pid, sizepid)
  * Zalando (link, pid)

### Add to monitor quicktask
You can create an add to monitor quicktask by adding quicktaskType=monitor to the quicktask url

### Country
Some sites support the country parameter in the quicktask, the country is not mandatory, you can add it with this format country=<country> with the country being lowercase

**Sites supporting the country parameter**
 * Amazon
 * Awlab
 * Footpatrol 
 * JDSports
 * NBSklep
 * Size

 ### Additional parameters
We also support other optional additional parameters such as:
 * method, used to set payment method of the task, the value should match the payment method name in the PanAIO GUI
 * mode, used to set mode of the task, the value should match the payment mode in the PanAIO GUI
 * quantity, used to sent quantity of the item
 * priceLimit, used only on amazon to specify the maximum of an item, if the item price should be less than 100€ for example priceLimit must be set to 100
 * details, used only on amazon to specify an offerid this must be used with Fast mode
