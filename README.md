# Gestão de Pendências - Inventário

Projeto React (Vite) pronto para rodar em um navegador de verdade — fora do
preview do Claude — para que o upload de imagens (galeria/câmera) funcione
normalmente no celular.

## Opção 1 — Testar rápido no CodeSandbox (sem instalar nada)

1. Acesse **codesandbox.io** no computador.
2. Clique em **"Create"** → **"Import Project"** (ou arraste este `.zip` direto
   para o painel do CodeSandbox — ele reconhece e importa automaticamente).
3. Aguarde a instalação automática das dependências.
4. O CodeSandbox gera um link público (algo como
   `https://xxxxx.csb.app`) — abra esse link no navegador do celular
   (Chrome/Safari) e teste o "Anexar imagem" normalmente.

## Opção 2 — Publicar de verdade (Vercel, gratuito)

1. Crie uma conta gratuita em **github.com**, se ainda não tiver.
2. Crie um repositório novo e suba esta pasta inteira (pelo site do GitHub,
   em "Add file" → "Upload files", ou usando `git push` se preferir).
3. Acesse **vercel.com**, crie uma conta gratuita e conecte com o GitHub.
4. Clique em **"Add New Project"**, selecione o repositório que você subiu.
5. O Vercel detecta automaticamente que é um projeto Vite — não precisa
   mudar nenhuma configuração. Clique em **"Deploy"**.
6. Em ~1 minuto você recebe um link público definitivo
   (ex: `gestao-pendencias-inventario.vercel.app`), que pode ser aberto de
   qualquer celular ou compartilhado com a equipe.

## Rodando localmente (opcional, se tiver Node.js instalado)

```bash
npm install
npm run dev
```

Abre em `http://localhost:5173`.

## Importante sobre os dados

Este app ainda guarda as pendências apenas na memória do navegador (não há
banco de dados). Ou seja, ao fechar a aba ou atualizar a página, os dados
cadastrados são perdidos. Isso é independente de onde o app está hospedado —
é preciso conectar um banco de dados (ou uma planilha/Google Sheets, por
exemplo) para os dados persistirem de verdade entre sessões e usuários. Se
quiser, posso ajudar a planejar essa parte depois.
