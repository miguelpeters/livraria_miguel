# Atividade 6 - Melhorando a Segurança do CRUD com Prepared Statements

Nessa atividade será apresentado o Prepared Statements e como ele pode ser usado
para a segurança de um usuário 

## O que é o Prepared Statements?

é uma forma de executar comandos SQL utilizando 
uma estrutura de consulta previamente definida
e parâmetros separados dos dados que serão utilizados na consulta. 
Em vez de construir uma string SQL misturando comandos SQL 
com informações recebidas do usuário,
utilizamos marcadores, normalmente "?"

## Por que não devemos colocar diretamente dados do usuário no SQL?

O código pressupõe que o usuário sempre fornecerá um número válido. 
Entretanto, um usuário mal-intencionado pode modificar manualmente esses parametros.
Quando uma aplicação junta uma entrada do usuário diretamente em uma consulta SQL, 
existe o risco de que essa entrada seja interpretada como parte do próprio comando SQL.
Essa vulnerabilidade é conhecida como SQL Injection.

## O que é Sql Injection?

SQL Injection é uma vulnerabilidade que ocorre quando informações controladas 
pelo usuário são incorporadas de maneira insegura a comandos SQL.
O objetivo de um ataque de SQL Injection pode ser, dependendo da vulnerabilidade,
consultar informações indevidas, alterar dados e excluir registros

## No que o o 