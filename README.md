# 🔐 Backend – Sistema de Autenticação (C# / .NET)

API REST desenvolvida em C# usando .NET para cadastro, login e recuperação de senha de usuários via e-mail.

## Sobre o projeto
Backend criado para gerenciar usuários, autenticação e envio de e-mail para recuperação de senha. Estrutura organizada em camadas, seguindo boas práticas de separação de responsabilidades e padrão Repository/Service.

## Tecnologias
- C# / .NET  
- Entity Framework Core  
- MySQL  
- SMTP para envio de e-mail  
- Arquitetura em camadas  

## Funcionalidades
- Cadastro de usuários   
- Login com validação de credenciais  
- Recuperação de senha via e-mail  

## Estrutura do projeto

- **Controllers** → São responsáveis por receber as requisições da API e chamar os services. Eles não fazem nenhuma lógica, apenas direcionam a ação.  
- **Services** → Aqui fica a lógica do sistema, como validar usuários no login, processar o cadastro e enviar e-mails de recuperação de senha.  
- **Repository** → É a parte que conversa direto com o banco de dados. Tudo que precisa salvar, buscar ou atualizar passa por aqui, mantendo o restante do código limpo.  
- **Models / Entities** → São as entidades do sistema, como Usuário, e também os modelos usados para passar informações entre camadas.  
- **Data / Context** → Contém o DbContext do Entity Framework e a configuração do banco de dados.  
- **Common** → Classes e utilitários que uso em várias partes do projeto, como constantes, mensagens de erro ou funções simples que ajudam no código.  
- **appsettings.json** → Aqui ficam as configurações principais do projeto, como a conexão com o banco, o SMTP para envio de e-mail e outras variáveis que a aplicação precisa.
  - Outras variáveis da aplicação  

---
