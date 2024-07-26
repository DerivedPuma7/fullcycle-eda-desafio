### EDA - Event Driven Architecture - Desafio

## Seting up environment
- Start containers
  > docker compose up -d

- Make sure to create Apache Kafka topics
  - go to http://localhost:9021 for Control Center or http://localhost:8000 for Kafka Ui  
    > create both 'balances' and 'transactions' topics, with default configs

## Start application
- Access go container for both services and run main.go
  - wallet core
    > docker exec -it wallet-core bash
    > go run cmd/walletcore/main.go
  - balances
    > docker exec -it wallet-balances bash
    > go run cmd/balances/main.go
