<div class="section-left-align">
<p class>- Exemplo browser </p>

<p class="fragment">- Browser escolhe qual será a proximo tarefa a ser executada </p>

<p class="fragment">- Toda execução de tarefa tira o controle do browser </p>

<p class="fragment">- Outros tarefas esperam ser chamadas uma de cada vez </p>

<p class="fragment">- uma tarefa que não termina trava todos as outras </p>

<p class="fragment">- A engine do JS executa uma tarefa por vez, quando pedida </p>

<p class="fragment">- Pedida por quem? </p>
</div>

<aside class="notes">
    A engine JS sempre está hospedada em algum ambiente, seja browser, em Node.js, e outros, mas todos eles possuem em comum, um mecanismo que possibilitam executar funções em sequencia, invocando a engine e dizendo para esta executar a função, isso é chamado de event loop.
    A engine JS não tem noção de tempo seguencia, ela apenas executa o que o ambiente pediu a ela.
</aside>
