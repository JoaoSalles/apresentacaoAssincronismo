<pre>
    <code class="hljs" data-trim data-line-numbers>
        listen( "click", handler );
        function handler() {
            setTimeout( request, 500 );
        }

        function request(){
            ajax( "http://some.url.1", response );
        }

        function response(text){
            if (text == "hello") {
                handler();
            }
            else if (text == "world") {
                request();
            }
        }
    </code>
</pre>

<aside class="notes">
    Apesar de termos nosso código modificado para termos uma visão síncrona e sem as famosas indentações, o código continua suscetível ao callback hell, o motivo é que o callback hell é relacionado mais ao pulo de uma função para outra, isso é o callback hell.
</aside>