# JBiHashMap

<b>JBiHashMap</b> is a custom implementation of the HashMap class provided by Java. 
This implementation provides most of all of the optional map operations, and permits null values and the null key.

The advantage of using this particular implementation allows the user to access data from <b>both</b> the directions, either by <b>key</b> or by <b>value</b>.


## How to use
To <b>initialize</b> a BiHashMap, you can call the standard constructor

<code>
BiHashMap<String, String> bhm = new BiHashMap<String, String>();
</code>

or define an initial capacity

<code>
BiHashMap<String, String> bhm = new BiHashMap<String, String>(10);
</code>
 
or defining both initial capacity and loadFactor

<code>
BiHashMap<String, String> bhm = new BiHashMap<String, String>(10, 0.75);
</code>

You can add items by simply calling the <b>put</b> method

<code>
bhm.put("Hello", "World!");
</code>

and you can <b>remove</b> them either by <b>key</b>

<code>
bhm.removeByKey("Hello");
</code>

or by <b>value</b>

<code>
bhm.removeByValue("World");
</code>

You can also retreive the <b>value</b> by <b>key</b>

<code>
String world = bhm.getValueByKey("Hello");
</code>

or you can retrieve the <b>key</b> by the <b>value</b>

<code>
String hello = bhm.getKeyByValue("World");
</code>

for further information please check out the javadoc
