<pre>
    <code class="hljs" data-trim data-noescape data-line-numbers>
function bar() {
	// `foo(..)` terminou executar isso
}

function oopsBar() {
	// oops, algo deu errado em `foo(..)`
    // executar isso
}

var p = foo( 42 );

p.then( bar, oopsBar );
    </code>
</pre>
<aside class="notes">
ou mais simples ainda
</aside>