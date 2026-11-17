# MLDDS 4.1.18

- Recupera a primeira abertura da minuta em qualquer operação sem exigir mudança nos resultados de uma pesquisa idêntica.
- Reavalia minutas abandonadas quando o histórico comprova que não houve Save. Gravações confirmadas ou incertas continuam protegidas.
- Renova a leitura dos controles quando o DDS recria a interface e preserva o Save confirmado se houver falha posterior de navegação.
- Corrige o Confirmar após Parar após atual, preservando a retomada da fila sem repetir Save.
- Usa o mesmo prazo de captura na retomada e na preparação normal, aguardando a origem comprovada.
- Evita a ativação da janela principal do DDS ao fechar modais no processamento em segundo plano.
- Mantém a conferência de minuta, rota, operação, destinos, classificação, KM e confirmação da gravação.

Extensão exigida: 2.0.13.
A continuidade também reconcilia a Pesquisa após falha de avanço, sem repetir gravações confirmadas, e mantém a operação esperada durante a renovação da janela.
