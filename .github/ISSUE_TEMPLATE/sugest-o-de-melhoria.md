---
name: Sugestão de Melhoria
about: Create a report to help us improve
title: ''
labels: documentation
assignees: clascleo

---

**Describe the bug**
Ao usarmos o método GET, fazendo uso do código de acesso (token) de um usuário comum (que não seja administrador), a API retorna com todas as informações de todos os usuários cadastrados, fazendo com que haja falha na segurança.

**To Reproduce**
Steps to reproduce the behavior:
1. Escolha opção de verbo (get) CT03 - 200 - listar usuários cadastrados
2. Clique em "send"
3. Retornará como resposta uma lista com todos os dados dos usuários cadastrados.


**Expected behavior**
Acredito que uma lista com a quantidade de usuários seria suficiente para uma consulta onde quem o faz não é um Administrador, podendo também ser uma rota exclusiva para administrador, pois evitaria uma exposição de dados desnecessária.

Imagem da tela:

![Get usuários (postman)](https://user-images.githubusercontent.com/109304734/188415219-070d4e6f-06be-4bc4-810f-cd14da052424.png)
