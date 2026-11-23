# MLDDS 4.1.19

- Alteração de Ciclo aceita lotes grandes e exibe progresso, previsão e resultados por minuta.
- A Pesquisa descarta cedo a grade antiga durante a troca de rota. A nova grade e a identificação da minuta aberta continuam obrigatórias.
- Um mesmo ID logístico pode incluir várias minutas distintas. Cada uma tem checkpoint e confirmação de Save próprios.
- Minutas já conformes saem da fila após conferência do ciclo. A tela e o Excel mostram a transição e os motivos de revisão.
- A importação reconhece o cabeçalho Ciclo PM - Pré Fatura (AM/PM). O início de Pedágios verifica componentes e permissões antes da primeira linha.
- Extensão exigida 2.0.13.
