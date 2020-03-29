<pre>
    <code class="hljs" data-trim data-noescape data-line-numbers="2,4,9,12,14">
var x = 0;
function *foo() {
    x++;
    yield; // pause!
    console.log( "x:", x );
}

// construct an iterator `it` to control the generator
var it = foo();

// start `foo()` here!
it.next();
x;                        // 1
it.next();        
    </code>
</pre>
<aside class="notes">
    generator parecem muito com funções normais, com acrescimo de * e yield
    Para executar o generator, precisamos do iterator e usamos next navegar o generator
    Iterable é um objeto iteravel, como Array e Maps, é possivel criar objetos iteraveis.
</aside>