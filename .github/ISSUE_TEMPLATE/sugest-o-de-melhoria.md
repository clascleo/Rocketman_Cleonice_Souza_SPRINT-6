---
name: Sugestão de Melhoria
about: Create a report to help us improve
title: Melhoria
labels: documentation
assignees: clascleo

---

**Describe the bug**
Na descrição anterior, relatei um problema (eu considero), onde um usuário comum pode consultar a lista de usuários cadastrados e visualiza não somente a quantidade, mas também todos os dados de cada um.
Porém o problema vai além de visualizar, essa mesma pessoa que esta fazendo a consulta (sem o código de acesso de administrador), consegue também fazer uma edição nos dados de qualquer usuário cadastrado.

**To Reproduce**
Steps to reproduce the behavior:
1.Escolha opção de verbo (get) CT03 - 200 - listar usuários cadastrados;
2.Clique em "send";
3.Retornará como resposta uma lista com todos os dados dos usuários cadastrados.
4.Escolha qualquer usuário da lista, copie e cole no "body" da sua requisição;
5.O ID do usuário escolhido ficará na barra de endereço da requisição;
6.Use o verbo "put", e edite os dados do usuário;
7.Clique em "send" ;
8.Note que a mensagem de retorno é "Registro alterado com sucesso".

**Expected behavior**
O esperado nesse caso seria um retorno com uma mensagem de rota exclusiva para administrador, com status code 403.
 
Veja:

![Put usuários Postman](https://user-images.githubusercontent.com/109304734/188421289-a7925b7a-fb7d-4532-ad7e-95a37dffbd05.png)
