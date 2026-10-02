# BrisaSensors

Superprojeto Git do BrisaSensors, sistema fictício de monitoramento da qualidade do ar em ambientes internos de escritórios, escolas, clínicas e academias. É o ponto de entrada do sistema: cada serviço tem repositório próprio, e este os reúne.

| Serviço | Repositório | Responsabilidade |
|---|---|---|
| Gestão de dispositivos | [brisasensors-device-management](https://github.com/sidartaoss/brisasensors-device-management) | Inventário e ciclo de vida dos dispositivos: comissionamento, configuração remota, calibração e descomissionamento |
| Ingestão | [brisasensors-ingestion](https://github.com/sidartaoss/brisasensors-ingestion) | Recebimento das leituras via MQTT, HTTP e LoRaWAN, validação e normalização em um evento canônico |
| Monitoramento do ar | [brisasensors-air-monitoring](https://github.com/sidartaoss/brisasensors-air-monitoring) | Histórico e valor atual por ambiente e alertas de CO₂ acima do limite |

As fronteiras entre os serviços e as alternativas descartadas estão no [estudo de caso](https://github.com/sidartaoss/fronteiras-de-microsservicos#7-estudo-de-caso-brisasensors) do guia Fronteiras de Microsserviços.
