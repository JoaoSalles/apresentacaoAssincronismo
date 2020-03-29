<pre>
    <code class="hljs" data-trim data-noescape data-line-numbers>
var a = 20;
function bar() {
    a = a * 2;
};

function foo() {
    a = a + 1;
};

ajax("http://some.url.1", foo );
ajax("http://some.url.2", bar );
    </code>
</pre>
