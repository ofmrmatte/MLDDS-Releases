# MLDDS 4.1.14

- Adiciona Alteração de Ciclo por planilha, com AM/PM, restauração das tabelas, igualdade de KM, recálculo e confirmação do Save, preservando as cidades.
- Permite descartar a planilha, continuar após conferência e pular minutas cujo ciclo já está correto.
- Compartilha o fluxo de roteirização entre Operação e Cadastro Méli, incluindo Maps/Imgur e correção da operação da minuta.
- Estabiliza a seleção do motorista, confirma CPF e operação e preserva o CPF já confirmado nas retomadas.
- Reforça a confirmação dos modais DDS e o processamento em segundo plano.
- Corrige a exclusão das regras, a projeção das regras ativas e a validação da UF após a troca da operação.
- Mantém a captura do Mercado Livre com a janela interna oculta.

O instalador preserva dados, regras, filas e credenciais existentes. Manifesto assinado com a mesma chave confiada pela 4.1.13. Captura exigida: 2.0.12.

Validação: compilação sem avisos ou erros; 1.598 testes do motor, 179 da shell, 246 da interface e 94 da captura aprovados. Os 31 testes que exigem duas planilhas históricas permanecem pendentes por ausência dos arquivos; a suíte completa não é declarada integralmente aprovada. O histórico operacional da dev.23 confirma gravações após a troca da operação.
