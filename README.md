# Work-Queues

Essa atividade é referente ao segundo exercício realizado utilizando o RabbitMQ. Não muito diferente da primeira, nesta atividade também terá um produtor e um consumidor. Porém, os produtores irão ter o papel de "trabalhadores" e os consumidores serão as "tarefas". Assim, foram inicializados diferentes arquivos dessas duas estruturas.

## Ferramentas utilizadas

RabbitMQ, Pycharm, Erlang

## Processo de execução

Assim como na primeira atividade, foram instaladas as ferramentas necessárias e depois foi visto o tutorial indicando o passo a passo de como tudo deveria ser feito. Portanto, foram criados os arquivos "new_task.py" e "worker.py", responsáveis por fazer a comunicação entre si. Dessa forma, foram iniciados através do terminal vários "workers", que receberiam as "tasks" vindas de uma fila, que recebia as mensagens criadas pelo arquivo "new_task.py". Desse modo, foram feitos diversos testes por meios desses dois arquivos.

## Resultado esperado

Depois do processo de execução, é esperado que as "tasks" sejam postas em uma espécie de fila no RabbitMQ, que seriam pegas pelos "workers" de acordo com a ordem em que eles foram iniciados no terminal. Ou seja, o primeiro "worker" receberia a primeira "task", o segundo "worker" receberia a segunda "task", de maneira que a task não seria compartilhada com outros "workers", logo, ela é única e exclusiva. Dessa forma, as tasks ficam em um ciclo contínuo, sendo recebidas seguindo a ordem dos "workers".
