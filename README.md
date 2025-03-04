# PanAIO quicktask documentation

### Quicktask Structure

<pre><code>
 https://www.panaio.com/quicktask?link={productLink}
 
</code></pre>

 
****site = Asos**** <br>
****productLink = https://www.asos.com/nike/nike-p-6000-trainer-in-metallic-silver-and-red/prd/207050743**** <br>


### Examples of quicktask
<pre> https://www.panaio.com/quicktask?link=https%3A%2F%2Fwww.asos.com%2Fnike%2Fnike-p-6000-trainer-in-metallic-silver-and-red%2Fprd%2F207050743 </pre>


### Site parameter
***Using the site parameter is now deprecated and not suggested anymore, just specify the link and the bot will get the site on its own, please note that if you specify a pid/SKU you still need to supply a site since the bot cannot detect the site from just the pid/sku***
***The brackets next to the sites indicate that the parameters specified can be entered instead of the productLink***

 **Values to insert in the variable site**
  * About You (link, pid)
  * Adidas (link, pid)
  * Alternate (link, pid)
  * Amazon (link, pid)
  * Asics (link, pid)
  * Asos (link, pid)
  * Auchan (link, pid)
  * Awlab (link, pid)
  * Boozt (link, pid)
  * Breuninger (link, pid)
  * Caseking (link, pid)
  * Cisalfa (link)
  * Courir (link, pid, sizepid)
  * Crocs (link, pid) pid format is pid-color
  * Disney (link, pid)
  * End Clothing (link, pid)
  * Fnac (link, pid)
  * Footlocker (link, pid)
  * Footpatrol (link, pid, sizepid)
  * Footshop (link, pid)
  * Funko Europe (link)
  * Gamestop (link, pid)
  * Here Store (link, pid)
  * H&M (link, pid)
  * JDSports (link, pid, sizepid)
  * JDSports East (link) this is site name for jdsports pl,sk,hu,ro,lt
  * JoueClub (link, pid)
  * Kickz (link, pid)
  * LVR (link, pid)
  * Micromania (link, pid)
  * Modivo (link, pid)
  * Mueller (link, pid)
  * Myntra (link, pid)
  * NBSklep (link, pid) this is site name for newbalance cz,pl,sk,hu
  * New Balance (link, pid) (add style after pid or url in this format pid:style)
  * Nike (link, pid) (pid can be both productId and sku)
  * PRM (link, pid)
  * QueueIT (link)
  * Rinascente (link, pid)
  * SecuTix (link)
  * Shopify (link)
  * Size (link, pid, sizepid)
  * Snipes (link, pid)
  * Solebox (link, pid)
  * TheHipStore (link, pid, sizepid)
  * Toys Center (link, pid)
  * Zalando (link, pid)

### Country
Some sites support the country parameter in the quicktask, the country is not mandatory, you can add it with this format country=<country> with the country being lowercase

**Sites supporting the country parameter**
 * Amazon
 * Awlab
 * Footpatrol 
 * JDSports
 * JDSports East
 * NBSklep
 * Size

 ### Additional parameters
We also support other optional additional parameters such as:
 * method, used to set payment method of the task, the value should match the payment method name in the PanAIO GUI
 * mode, used to set mode of the task, the value should match the payment mode in the PanAIO GUI
 * quantity, used to sent quantity of the item
 * priceLimit, used only on amazon to specify the maximum of an item, if the item price should be less than 100€ for example priceLimit must be set to 100
 * details, used only on amazon to specify an offerid this must be used with Fast mode

Other parameters might still be supported even if undocumented, please open a ticket in our discord support server if you have some specific questions https://discord.gg/AvgQ2EMW
