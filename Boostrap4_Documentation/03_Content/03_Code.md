

Code
Documentation and examples for displaying inline and multiline blocks of code with Bootstrap.

All the tools your team needs in one place. Slack: Where work happens.
ads via Carbon
Inline code
Wrap inline snippets of code with <code>. Be sure to escape HTML angle brackets.

For example, <section> should be wrapped as inline.
Copy
For example, <code>&lt;section&gt;</code> should be wrapped as inline.
Code blocks
Use <pre>s for multiple lines of code. Once again, be sure to escape any angle brackets in the code for proper rendering. You may optionally add the .pre-scrollable class, which will set a max-height of 350px and provide a y-axis scrollbar.

<p>Sample text here...</p>
<p>And another line of sample text here...</p>
Copy
<pre><code>&lt;p&gt;Sample text here...&lt;/p&gt;
&lt;p&gt;And another line of sample text here...&lt;/p&gt;
</code></pre>
Variables
For indicating variables use the <var> tag.

y = mx + b
Copy
<var>y</var> = <var>m</var><var>x</var> + <var>b</var>
User input
Use the <kbd> to indicate input that is typically entered via keyboard.

To switch directories, type cd followed by the name of the directory.
To edit settings, press ctrl + ,
Copy
To switch directories, type <kbd>cd</kbd> followed by the name of the directory.<br>
To edit settings, press <kbd><kbd>ctrl</kbd> + <kbd>,</kbd></kbd>
Sample output
For indicating sample output from a program use the <samp> tag.

This text is meant to be treated as sample output from a computer program.
Copy
<samp>This text is meant to be treated as sample output from a compute
