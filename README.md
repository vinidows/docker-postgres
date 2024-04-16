# docker-postgres
Comando para criação de um container com banco de dados postgres com o uso do docker


docker container run --name Desafio01 -d -p 5434:5434 -e POSTGRES_DB=curso_docker -e POSTGRES_USER=docker_usr -e POSTGRES_PASSWORD=docker_pwd postgres

docker container run <-- é usado para criação de um container em cima de uma imagem
-- name NOME <-- é usado para escolher o nome do container o nome dele ser colocado logo em seguida
-d <-- mostra para o Deamon que o container é um teste e deve ser continuo
-p 5434:5430 <-- é para escolher a porta de saido do container 5434: é a porta e 5430 é a subporta (Modificado somente para o exemplo)
-e <-- é usado para podermos adicionar as variaveis da imagem e devem sempre estar antes da variavel
postgres <-- e o nome da imagem e sempre deve estar no final.
POSTGRES_DB=NOMEDOBANCO
POSTGRES_USER=NOMEDOUSUARIO
POSTGRES_PASSWORD=SENHADOBANCO
