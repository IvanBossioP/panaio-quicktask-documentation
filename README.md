# PanAIO QuickTask Documentation

## Supported sites
  * [Asos](#Asos)
  * [Awlab](#Awlab)
  * [Defshop](#Defshop)
  * [Footshop](#Footshop)
  * [LDLC](#Ldlc)
  * [Mesh](#Mesh)
  * [Revolve](#Revolve)
  * [Rinascente](#Rinascente)
  * [Zalando](#Zalando)
------------------------------------
### Asos
<h4> FORMAT: http://localhost:5080/query?{pid,link,size,site} </h4>

**The object must be urlencoded**

* The size field can contain only one size (size=7)
* The size format must be in UK
* The pid field must contain the id of the size

EXAMPLE:
<pre> http://localhost:5080/query?site=Asos&link=https%3A%2F%2Fwww.asos.com%2Fit%2Fnike%2Fnike-air-max-270-essential-sneakers-bianche%2Fprd%2F21390440%3Fclr%3Dbianco%26colourwayid%3D60163237%26SearchQuery%3Dnike&size=7&pid=21390531 </pre>


### Awlab
<h4> FORMAT:  http://localhost:5080/base64?data="{{pid,link,size,site}}" </h4>
( pid, link, size[ ] ) 

**The object must be converted to a Json string and then to base64**

* The size field can contain more sizes (size=7,4,4.5,5.5)
* The size format must be in US

EXAMPLE:
<pre> http://localhost:5080/base64?data=eyJzaXRlIjoiQXdsYWIiLCJsaW5rIjoiaHR0cHM6Ly9lbi5hdy1sYWIuY29tL21lbi9zaG9lcy9iYXNrZXQvbmlrZS1zYi1ibGF6ZXItdmFwb3ItQVdfMjIxMjIyMkEuaHRtbD9jZ2lkPW1lbl9zaG9lc19iYXNrZXRiYWxsc2hvZXMmZHd2YXJfQVdfXzIyMTIyMjJBX2NvbG9yPTgwNDE2MjMiLCJzaXplIjpbIjciXSwicGlkIjoiQVdfMjIxMjIyMkFfODA0MTYyMyJ9 </pre>


### Defshop
<h4> FORMAT: http://localhost:5080/query?{pid,link,size,sizeId,site} </h4>

**The object must be urlencoded**

**The country of the supported site is the German one 'https://www.def-shop.com/'**

* The link field must contain only the the German link <pre>https://www.def-shop.com/nike-w-air-max-90-sneakers-white-arctic-punch-barely-green.html</pre> We don't accept another region link format <pre>https://www.def-shop.com/it/p/nike-air-max-270-ess--sneakers-nero-DM2462001.html</pre>
* The size field can contain only one size (size=38)
* The size format must be in EU
* The pid field must contain the product pid
* The sizeId field must contain the id of the size

EXAMPLE:
<pre> http://localhost:5080/query?site=Defshop&link=https%3A%2F%2Fwww.def-shop.com%2Fnike-w-air-max-90-sneakers-white-arctic-punch-barely-green.html&size=40&pid=824176&sizeId=8195379 </pre>


### Footshop
<h4> FORMAT: http://localhost:5080/query?{pid,link,size,sizeId,site} </h4>

**The object must be urlencoded**

* The size field can contain only one size (size=7)
* The size format must be in US
* The pid field must contain the product pid
* The sizeId field must contain the id of the size

EXAMPLE:
<pre> http://localhost:5080/query?site=Footshop&link=https%3A%2F%2Fwww.footshop.it%2Fit%2Fscarpe-e-sneaker-da-uomo%2F114958-nike-air-force-1-07-premium-coconut-milk-atomic-orange-fuel-orange.html&size=7&pid=114958&sizeId=728683 </pre>


### LDLC
<h4> FORMAT: http://localhost:5080/query?{pid,link,site} </h4>

**The object must be urlencoded**

EXAMPLE:
<pre> http://localhost:5080/query?pid=AR201601220127&link=https%3A%2F%2Fwww.ldlc.com%2Ffiche%2FPB00203250.html&site=LDLC </pre>


### Mesh
* JDSports
* Footpatrol
* Size
* TheHipStore

<h4> FORMAT: http://localhost:5080/query?{pid,sizeId,site} </h4>

**The object must be urlencoded**

EXAMPLE:
<pre> Test </pre>

### Revolve
<h4> FORMAT: http://localhost:5080/query?{pid,link,size,site} </h4>

**The object must be urlencoded**

* The size field can contain only one size (size=7)
* The size format must be in US

EXAMPLE:
<pre> http://localhost:5080/query?site=Revolve&link=https%3A%2F%2Fwww.revolve.com%2Fsuperga-2750-cotu-classic-sneaker%2Fdp%2FSERG-WZ33%2F%3Fd%3DWomens%26srcType%3Dhp_recs_viewed&size=6&pid=SERG-WZ33 </pre>


### Rinascente
<h4> FORMAT: http://localhost:5080/query?{pid,link,size,site} </h4>

**The object must be urlencoded**

* The size field can contain only one size (size=38)
* The size format must be in EU
* The pid field must contain the id of the size

EXAMPLE:
<pre> http://localhost:5080/query?site=Rinascente&link=https%3A%2F%2Fwww.rinascente.it%2Fit%2Fitem%2Fadidas-originals-sneakers-stan-smith-in-pelle-0223578800001&size=38&pid=17231462 </pre>


### Zalando
<h4> FORMAT:  http://localhost:5080/base64?data="{{pid,link,size,site}}" </h4>
( pid[ ], link[ ], size[[ ]] ) 

**The object must be converted to a Json string and then to base64**

* The size field can contain multiple sizes (size=7,8,8.5)
* The size format must be in US

EXAMPLE:
<pre> http://localhost:5080/base64?data=eyJzaXRlIjoiWmFsYW5kbyIsImxpbmsiOlsiaHR0cHM6Ly93d3cuemFsYW5kby5pdC9qb3JkYW4tYWlyLWpvcmRhbi0xLW1pZC1zbmVha2Vycy1hbHRlLXdoaXRlZ3ltLXJlZGJsYWNrLWpvYzEybjAwMS1hMjEuaHRtbCJdLCJwaWQiOlsiSk9DMTJOMDAxLUEyMTAwNzAwMDAiXSwic2l6ZSI6W1siNyJdXSwiaW1hZ2UiOlsiaHR0cHM6Ly9pbWcwMS56dGF0Lm5ldC9hcnRpY2xlL3NwcC1tZWRpYS1wMS8wMDljMzU4ZmU0MTI0MzIzODE1MTUzMDU5NTlhNjE1Yi84YTg2OGRlZjI4OGE0ODE0ODNlMWU5ZTdiYmM5MDg4ZC5qcGc/aW13aWR0aD0xMDMiXX0=
</pre>
