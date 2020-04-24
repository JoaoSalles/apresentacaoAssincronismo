### Ambiente javascript

<div class="section-left-align">
<p class="fragment">- A engine JS sempre está hospedada em algum ambiente</p>

<p class="fragment">- Ambiente cria uma fila de tarefas</p>

<p class="fragment">- Ambiente pede para a engine JS executar as tarefas</p>

<p class="fragment">- Isso é chamado de Event loop</p>

</div>

<aside class="notes">
    A engine JS sempre está hospedada em algum ambiente, seja browser, em Node.js, entre outros. Contudo, todos os ambientes possuem algo em comum, um mecanismo que possibilita executar pedaços do programa ao longo do tempo. O ambiente assim cria uma fila de tarefas e dita para a engine o que executar, isso é chamado de event loop. A engine em si não tem noção de tempo, ela simplesmente executa o pesado de código que é pedido para ela.
</aside>