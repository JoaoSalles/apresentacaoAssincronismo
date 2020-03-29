<pre>
    <code class="hljs" data-trim data-line-numbers="5,7,9-15">
        # array de eventos
        var eventLoop = [];   
        var event;
        # loop infinito
        while (true) {
            # caso haja eventos/tick
            if (eventLoop.length > 0) {
                # remove primeiro elemento do array e retorna ele
                event = eventLoop.shift();
                try {
                    event();
                }
                    catch (err) {
                    reportError(err);
                }
            }
        }
    </code>
</pre>

<aside class="notes">
    Cada execução do loop é chamado de tick(instante), e em cada tick um evento/message da fila é removido e executado, seguindo a ordem de chegada.
</aside>
