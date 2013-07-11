jquery-clockpick-timepicker-plugin
==================================

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
<tr bgcolor="#dddddd">
<td align="right" valign="top"><h3>Using bgIframe plugin </h3></td>
<td><p>To account for the notorious IE6 select menu show-through issue, a popular jQuery plugin called <a href="http://jquery.com/plugins/files/bgiframe-2.1.zip">bgIframe</a> is frequently used. ClockPick offers support for this plugin by setting a configuration variable useBgiframe = true. By doing this, ClockPick calls the bgiFrame plugin at the right time so its divs are shown above any select menus that might be nearby.</p>
<p>First you will need to include the <a href="http://jquery.com/plugins/files/bgiframe-2.1.zip">bgIframe plugin</a>, somewhere afer your include of the jQuery library: <br>
<strong>&lt;script src=&quot;/path/to/bgiframeplugin.js&quot; type=&quot;text/javascript&quot;&gt;&lt;/script&gt; </strong></p>
<p>Then set the configuration variable when you call ClockPick:<strong><br>
$(&quot;.clockpick&quot;).clockpick({<br>
useBgiframe : true <br>
}); </strong> </p></td>
</tr>
</table>
<br>
<br>
