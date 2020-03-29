<pre>
    <code class="hljs" data-trim data-noescape data-line-numbers="9,10,15">
function foo() {
     return new Promise(function(resolve) {
           setTimeout(function() {
                resolve("test");
           }, 1000);
     });
}

async function main() {
    var text = await foo();
    // podemos continuar com código
    console.log(text);
}

main();
    </code>
</pre>
<aside class="notes">
    Com async function nos trocamos o * por async antes declaração de function
    e trocamos o yield por await. Assim temos um código escrito sincronamente
    com sua execução assincrona.
</aside>