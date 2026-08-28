# MLDDS 3.0.13

Release estável do MLDDS Automation.

- reconhece `ROTA NÃO REALIZADA`, recalcula somente a Venda, bloqueia a Compra e registra a observação com read-back;
- alinha a regra `+10% NÃO VISITADO` à referência v2J, mantendo Venda normal e Compra bloqueada;
- corrige recuperação de destinos, tabelas de frete, KM, próxima minuta e limpeza sem Save;
- aguarda a rota real no Google Maps, usa o KM exibido e mantém retry/read-back para Imgur e Link da Rota;
- melhora snapshot, deduplicação, interestadual, Desemboque e a classificação comprovada `VUC PP → VUC SDD`;
- extensão V2 2.0.9, ID produtivo preservado e sem instalação, recarga ou atualização automática pelo updater;
- upgrade preserva configurações, Combinados, auditoria e dados.

Commit fonte: `1835dd4cb3fcf40b17f4046bb5d7dea3916f4c8f`.

Authenticode: PENDING HARDENING. A integridade do canal atual é protegida por ECDSA P-256 e SHA-256.
