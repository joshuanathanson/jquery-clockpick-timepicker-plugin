jquery-clockpick-timepicker-plugin
==================================

<h4><a href="http://www.jnathanson.com/index.cfm?page=jquery/clockpick/ClockPick">Click here to view a ClockPick demo</a></h4>

<h2>Configuration</h2>
<table width="640" border="0" cellpadding="6" cellspacing="1">
<tr bgcolor="#f2f2f2">
<td align="right" valign="top"><h3>Basic</h3></td>
<td><p>After including the jQuery script in your html &lt;head&gt; block, include the jquery.clockpick.js file like so:<br>
&lt;script src=&quot;path/to/jquery.clockpick.js&quot;&gt;&lt;/script&gt;<br>
<br>
Include the clockpick css file:<br>
&lt;link rel=&quot;stylesheet&quot; href=&quot;path/to/clockpick.css&quot; type=&quot;text/css&quot;&gt;</p>
<p>Then in your $(document).ready block, simply add the following bit of code:</p>
<p><strong>$(&quot;#clockpick&quot;).clockpick();</strong></p>
<p>This assumes you are binding the plugin to an element with the id &quot;clockpick&quot;. You can certainly bind the plugin to any element that makes sense for your use. </p></td>
</tr>
<tr bgcolor="#dddddd">
<td align="right" valign="top" bgcolor="#dddddd"><h3>Adding parameters</h3></td>
<td><p>ClockPick takes two optional parameters:<br>
<strong>options</strong> (hash) - an object containing settings keys and their values<br>
<strong>callback</strong> (function) - a callback function to run after ClockPick is run</p>
<p>Example:</p>
<p><strong>$(&quot;#clockpick&quot;).clockpick({<br>
starthour : 6,<br>
endhour : 15,<br>
showminutes : false<br>
}, mycallback<br>
);
</strong><br>
</p></td>
</tr>
<tr bgcolor="#f2f2f2">
<td align="right" valign="top"><h3>Click target different <br>
than value field </h3></td>
<td><p>If you want to have the action on a different element than the time field, you would configure as below (like the &quot;click on clock&quot; demo).</p>
<p>Assuming the field you wish to have filled with the time, has the name 'myfieldname':</p>
<p><strong>$(&quot;.clockpick&quot;).clockpick({<br>
valuefield : 'myfieldname' <br>
});
</strong><br>
</p></td>
</tr>
</table>
<br>
<br>
