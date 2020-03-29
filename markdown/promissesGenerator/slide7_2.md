<pre>
    <code class="hljs" data-trim data-noescape data-line-numbers="2,4,10,18,21">
function foo() {
 return new Promise(function(resolve) {
   setTimeout(function() {
     resolve("test");
   }, 1000);
 });
}

function* main() {
 var text = yield foo();
 // podemos continuar com código
 console.log(text);
}

var it = main();

// start it all up!
var p = it.next().value;

p.then(function(data) {
 it.next(data);
}); 
    </code>
</pre>
<aside class="notes">
    Então temos, o primeiro yield retornando uma promise
    e o then da promise chamando o next com o resolve da promise
    Importante comentar que nosso exemplo apenas lida com 1 camada de promise
    existem libraries para lidar com mais
</aside>