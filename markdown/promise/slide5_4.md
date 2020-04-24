<pre>
   <code class="hljs" data-trim data-noescape data-line-numbers>
function foo(x) {
   // faz alguma coisa
 
   // constroe a promise
   return new Promise( function(resolve,reject){
       // eventually, call `resolve(..)` or `reject(..)`,
       // which are the resolution callbacks for
       // the promise.
   } );
}
   </code>
</pre>
<aside class="notes">
Foo seria algo nesse sentido, retornaria uma Promise
que invoca a função resolve caso sucesso ou
reject caso falha
Para registrarmos um evento de conclusão de promises usamos o then, que registra os eventos de fulfillment e rejection.
</aside>