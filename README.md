# MLDDS Releases

Canal público oficial de distribuição do MLDDS.

Este repositório contém somente artefatos e metadados necessários para instalação e atualização. Código-fonte, regras operacionais internas e configurações de ambiente permanecem no repositório privado de desenvolvimento.

## Fonte de verdade

O canal estável é descrito por:

```text
stable/manifest.json
```

O manifesto informa:

- versão estável atual;
- data da release;
- versão mínima suportada;
- URL do instalador;
- SHA-256 do artefato;
- assinatura do manifesto;
- notas de release;
- versão exigida da extensão;
- se a atualização é obrigatória.

Use o manifesto como fonte de verdade em vez de copiar a versão atual para vários arquivos que podem ficar desatualizados.

## Instaladores

As versões publicadas ficam em [GitHub Releases](https://github.com/ofmrmatte/MLDDS-Releases/releases).

Cada release deve corresponder ao artefato referenciado pelo manifesto estável.

## Integridade

Antes de promover uma nova versão para `stable`, confirme:

1. o instalador publicado é o artefato que passou pela homologação;
2. o SHA-256 do arquivo corresponde ao `sha256` do manifesto;
3. a assinatura do manifesto é válida;
4. `version`, `minimumSupportedVersion` e `extensionVersionRequired` são coerentes;
5. a URL do instalador aponta para a mesma versão publicada em GitHub Releases;
6. as notas descrevem a mudança efetivamente entregue.

Exemplo de conferência de SHA-256 no Windows:

```powershell
Get-FileHash .\MLDDS-Setup.exe -Algorithm SHA256
```

O nome local do instalador pode variar; compare o hash calculado com o valor do manifesto da release correspondente.

## Atualização da extensão

A extensão Chrome não deve ser considerada atualizada apenas porque o aplicativo foi instalado. Quando `extensionVersionRequired` mudar, siga a orientação da release para atualizar/recarregar a extensão manualmente.

## O que não deve entrar neste repositório

- código-fonte do MLDDS;
- credenciais;
- chaves privadas de assinatura;
- logs operacionais reais;
- configurações internas de clientes/operações;
- dados de rotas ou usuários;
- builds não homologados apresentados como estáveis.

O repositório de desenvolvimento permanece privado; este repositório funciona apenas como canal público e auditável de distribuição.
