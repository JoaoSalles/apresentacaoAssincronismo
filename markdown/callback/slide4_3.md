## Callbacks Hell
<pre>
    <code class="hljs" data-trim data-line-numbers>
        listen( "click", function handler(evt){
            setTimeout( function request(){
                ajax( "http://some.url.1", function response(text){
                    if (text == "hello") {
                        handler();
                    }
                    else if (text == "world") {
                        request();
                    }
                } );
            }, 500) ;
        } );
    </code>
</pre>

<aside class="notes">
    Quando pensamos em problemas com callbacks aninhados o que vem a cabeça é o famoso callback hel
</aside>