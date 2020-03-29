<pre>
    <code class="hljs" data-trim data-noescape data-line-numbers>
function bar(fooPromise) {
	// escuta `foo(..)` terminar
	fooPromise.then(
		function(){
			// `foo(..)` terminou agora executa
		},
		function(){
			// oops, algo deu errado em `foo(..)`
		}
	);
}
    </code>
</pre>
<aside class="notes">
sendo o corpo de Bar ou Baz
</aside>