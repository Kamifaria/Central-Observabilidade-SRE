# Central-Observabilidade-SRE

## O Cérebro de SRE da Arquitetura

Bem-vindo ao **Projeto 3: Central-Observabilidade**. Este projeto atua como o ***Cérebro de SRE (Site Reliability Engineering)*** responsável por monitorar todos os microsserviços da arquitetura, incluindo o **GatewayPagamentos** e o **CatalogoMicroservice**.

### Objetivo

Centralizar os dados de monitoramento, logs e traces, garantindo visibilidade total sobre a saúde, performance e disponibilidade de todo o ecossistema. Com o poder do Prometheus e do Grafana (e preparando terreno para o Stack LGTM inteiro), asseguramos a resiliência e a confiabilidade de cada transação de pagamento processada.

### O que tem na caixa?

1. **Prometheus**: Faz a coleta das métricas diretamente pelos endpoints de health-check e de métricas das APIs (`/health`).
2. **Grafana**: Fornece dashboards dinâmicos para visualização dos status das APIs (Uptime), uso de CPU e Memória, entre outras métricas de infraestrutura essenciais, com dashboards configurados automaticamente via Provisioning.

### Como Executar

Simplesmente inicie o Docker Compose:

```bash
docker-compose up -d
```

### Acessos

- **Prometheus UI**: [http://localhost:9090](http://localhost:9090)
- **Grafana**: [http://localhost:3000](http://localhost:3000) (Usuário: `admin` | Senha: `admin`)
