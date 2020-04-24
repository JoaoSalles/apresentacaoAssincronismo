<pre>
    <code class="hljs" data-trim data-noescape data-line-numbers>
function foo(x) {
    // faz alguma coisa

    return listener;
}

var evt = foo( 42 );

// evt.on( "completion", function(){
    // executa o proximo passo
// } );

// evt.on( "failure", function(err){
    // oops, algo deu errado em `foo(..)`
// } );

// evento vai ser executado dentro das funções
bar(evt)

baz(evt)

    </code>
</pre>
<aside class="notes">
Apesar de se comportarem como um evento, o evento de conclusão das promises não são estritamente eventos.
Para registrarmos um evento de conclusão de promises usamos o then, que registra os eventos de fulfillment e rejection.
</aside>