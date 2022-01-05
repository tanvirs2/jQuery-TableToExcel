# tableToExcel
Light weight jQuery plugin for export table to excel file


<h2>Demos</h2>

<p>Website and demo here:</p>

<p><a href="http://tanvirpro.com/" target="_blank">http://tanvirpro.com/all_project/jQueryTableToExcel</a></p>

<h2>Get started</h2>

<ul>
	<li>
	<p>Download the&nbsp;<a href="https://github.com/tanvirs2/jQuery-TableToExcel/archive/master.zip" rel="nofollow">last release</a>&nbsp;manually</p>
	</li>
</ul>

<p>Include&nbsp;<a href="https://code.jquery.com/jquery-3.2.1.min.js" rel="nofollow">jQuery</a>&nbsp;and the plugin.</p>

<pre>
<code>&lt;script src=&quot;https://code.jquery.com/jquery-3.2.1.min.js&quot;&gt;&lt;/script&gt;
&lt;script src=&quot;js/</code>jquery.tableToExcel.js<code>&quot;&gt;&lt;/script&gt;
</code></pre>

<p>Create Excel file form HTML table</p>

<p>Add plugin any table with CSS selector</p>

<pre>
<code>
<table>
    <tr>
        <th>Company</th>
        <th>Contact</th>
        <th>Country</th>
    </tr>
    <tr>
        <td>Alfreds Futterkiste</td>
        <td>Maria Anders</td>
        <td>Germany</td>
    </tr>
    <tr>
        <td>Centro comercial Moctezuma</td>
        <td>Francisco Chang</td>
        <td>Mexico</td>
    </tr>
    <tr>
        <td>Ernst Handel</td>
        <td>Roland Mendel</td>
        <td>Austria</td>
    </tr>
    <tr>
        <td>Island Trading</td>
        <td>Helen Bennett</td>
        <td>UK</td>
    </tr>
    <tr>
        <td>Laughing Bacchus Winecellars</td>
        <td>Yoshi Tannamuri</td>
        <td>Canada</td>
    </tr>
    <tr>
        <td>Magazzini Alimentari Riuniti</td>
        <td>Giovanni Rovelli</td>
        <td>Italy</td>
    </tr>
</table>
</code></pre>

<p>Apply the plugin to HTML table element on your HTML page and get excel file as like the table.</p>

<pre>
<code>&lt;script&gt;

    $(selector).</code>tblToExcel<code>();
    
    //... or
    
    $('button').click(function () {
        $('table').tblToExcel();
    });
    
&lt;/script&gt;
</code></pre>

<h2>Results</h2>

<p>Download xlx file</p>
<pre><code>  

	
</code></pre>
<h2>Settings</h2>

<ul>
<li>
	<p><strong>complete</strong>&nbsp;&mdash; Callback function trigged after the detection is completed</p>
<pre><code>  	
complete: function () {
	// ...
}
</code></pre>

</li>
</ul>

# Added custom name file tableToExcel
I just added some parameter for file name in jquery.tableToExcel.js at line 2, and line 36
<pre>
<code>&lt;script&gt;

	(function ($) {
		$.fn.tblToExcel = function (parameter) {
    
&lt;/script&gt;
</code></pre>


<pre>
<code>&lt;script&gt;

	link.download = parameter;
    
&lt;/script&gt;
</code></pre>
