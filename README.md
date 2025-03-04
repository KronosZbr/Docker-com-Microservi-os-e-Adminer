# Docker com Microserviços e Adminer

## Descrição

Este projeto configura um ambiente Docker com múltiplos microserviços, cada um com seu próprio banco de dados Postgres, utilizando Nginx como servidor web e Adminer para gerenciar os bancos de dados.

## Estrutura do Projeto

- **microservice1**: Nginx servindo conteúdo estático.
- **microservice2**: Nginx servindo conteúdo estático.
- **microservice3**: Nginx servindo conteúdo estático.
- **db1**: Banco de dados Postgres para o microservice1.
- **db2**: Banco de dados Postgres para o microservice2.
- **db3**: Banco de dados Postgres para o microservice3.
- **adminer**: Interface web para gerenciar os bancos de dados.

## Como rodar o projeto

1. **Clone o repositório:**
   ```bash
   git clone https://github.com/KronosZbr/Docker-com-Microservi-os-e-Adminer
   cd Docker-com-Microservi-os-e-Adminer
   ```

2. **Suba os containers:**
   ```bash
   docker-compose up -d
   ```

3. **Acesse os serviços:**
   - Microservice 1: [http://localhost:8001](http://localhost:8001)
   - Microservice 2: [http://localhost:8002](http://localhost:8002)
   - Microservice 3: [http://localhost:8003](http://localhost:8003)
   - Adminer: [http://localhost:8080](http://localhost:8080)

## Configurações de Banco de Dados

| Microserviço  | Usuário | Senha | Banco de Dados |
|---------------|--------|-------|----------------|
| microservice1 | user1  | pass1 | db1            |
| microservice2 | user2  | pass2 | db2            |
| microservice3 | user3  | pass3 | db3            |

## Parar os containers

Para parar todos os containers, use:
```bash
docker-compose down
```

## Contribuição

1. Faça um fork do projeto.
2. Crie uma branch (`git checkout -b feature/nova-feature`).
3. Commit suas alterações (`git commit -m 'Adiciona nova feature'`).
4. Faça o push para a branch (`git push origin feature/nova-feature`).
5. Abra um Pull Request.

## Licença

Este projeto está sob a licença MIT.

