## Callbacks alinhados
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
    cabeça é o callback hell
</aside>