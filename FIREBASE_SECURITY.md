# Segurança do Firebase — Tania Parfum Catálogo

Este catálogo lê dados públicos do Realtime Database do Firebase no projeto `taniaparfum233`.

## Arquivo de regras

As regras seguras estão no arquivo:

```text
firebase-database.rules.json
```

## Como aplicar no Firebase Console

1. Acesse o Firebase Console.
2. Entre no projeto `taniaparfum233`.
3. Vá em **Realtime Database**.
4. Abra a aba **Rules**.
5. Copie o conteúdo de `firebase-database.rules.json`.
6. Cole nas regras do Realtime Database.
7. Clique em **Publish**.

## O que estas regras fazem

- O catálogo pode ler produtos, preços, esgotados, carrossel e configurações públicas.
- O catálogo não consegue escrever no banco.
- Apenas usuários logados pelo sistema de Gestão conseguem alterar produtos, preços, carrossel, esgotados e configurações.
- Backups e dados internos ficam protegidos para usuários autenticados.
- A raiz do banco fica bloqueada por padrão.

## Caminhos públicos somente leitura

- `produtos_estaticos`
- `produtos_custom`
- `precos`
- `esgotados`
- `carrossel`
- `config`

## Caminhos privados

- `backup`

## Importante

Estas regras precisam ser publicadas manualmente no Firebase Console. O GitHub apenas guarda uma cópia segura das regras; ele não altera o Firebase automaticamente.
