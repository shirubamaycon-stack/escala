# Escala Noturna — instalar como app

## O que tem na pasta
- `index.html` — o app
- `manifest.json` — dados do app (nome, ícone, cor)
- `sw.js` — service worker (faz funcionar offline)
- `icon-192.png`, `icon-512.png`, `icon-512-maskable.png` — ícones

## Publicar no GitHub Pages (grátis)
1. Entre em github.com com a conta `shirubamaycon-stack`.
2. **New repository** → nome: `escala` → **Public** → Create.
3. Na página do repositório: **Add file → Upload files** → arraste os 6 arquivos → **Commit changes**.
4. **Settings → Pages** → em *Source* escolha **Deploy from a branch** → branch `main`, pasta `/ (root)` → **Save**.
5. Aguarde 1–2 minutos. O endereço fica:
   `shirubamaycon-stack.github.io/escala/`

## Instalar no celular
- **Android (Chrome):** abra o endereço → menu ⋮ → **Instalar app** / *Adicionar à tela inicial*.
- **iPhone (Safari):** abra o endereço → botão Compartilhar → **Adicionar à Tela de Início**.

Depois de instalado, abre em tela cheia, com ícone próprio, e funciona sem internet.

## Importante sobre os dados
Os dados ficam salvos **no aparelho** (não na nuvem). Cada celular tem a sua escala.
Use **Salvar backup (.json)** na aba Equipe de vez em quando, e **Restaurar backup**
para passar a escala para outro aparelho.

## Atualizar o app depois
Suba o `index.html` novo no GitHub e troque a linha 1 do `sw.js`:
`const CACHE='escala-v1';` → `'escala-v2'` (v3, v4...). Isso força o celular a baixar a versão nova.

