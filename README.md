# NutriConecta

Aplicacao web Spring MVC para conectar doadores de alimentos, instituicoes receptoras e controlar ofertas, itens, enderecos, solicitacoes e retiradas.

## Funcionalidades entregues

- Cadastro, listagem, edicao e exclusao de usuarios.
- Cadastro de enderecos vinculados a um usuario.
- Cadastro de alimentos.
- Cadastro de doacoes com doador, status e data de expiracao.
- Cadastro de itens de doacao com alimento existente ou novo alimento criado durante o cadastro.
- Solicitacoes de doacao por instituicoes.
- Aprovacao, rejeicao e cancelamento de solicitacoes.
- Registro de retiradas/entregas a partir de solicitacoes aprovadas.
- Historico visual por listas e tela de detalhes.

## Como executar

1. Crie o banco MySQL:

```sql
CREATE DATABASE dbnutriconecta CHARACTER SET utf8mb4 COLLATE utf8mb4_unicode_ci;
```

2. Ajuste usuario e senha no arquivo `src/main/resources/application.properties` ou use variaveis de ambiente:

```powershell
$env:DB_USER="root"
$env:DB_PASSWORD="sua_senha"
```

3. Rode o projeto:

```powershell
mvn spring-boot:run
```

4. Acesse:

```text
http://localhost:8080
```

O Hibernate esta configurado com `ddl-auto=update`, entao as tabelas sao criadas/atualizadas automaticamente.
