<pre>
    <code class="hljs" data-trim data-noescape data-line-numbers>
// constroe generator
function *foo(x) {
    return x * (yield “Qual seria o valor?”)
}

var it = foo(2)
// começa foo e para no yield
let res = it.next();
res.value                     // Qual seria o valor?

rest = it.next(2);                // Fornece valor
res.value;                        //  4    
    </code>
</pre>
<aside class="notes">
    O primeiro next para no primeiro yield que retorna “Qual seria o valor?”
    proximo next enviar o valor 2 que substitui  o yield
</aside>