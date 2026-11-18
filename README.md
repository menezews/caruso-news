# The CARUSO News

Jornal interno corporativo em formato de vídeo vertical, desenvolvido com React, Vite e Tailwind CSS.

## Desenvolvimento local

Requisitos:

- Node.js 22
- pnpm 10

```bash
pnpm install
pnpm dev
```

Para gerar a versão estática:

```bash
pnpm build
```

Os arquivos prontos para hospedagem serão gerados em `dist/`.

## Publicar no GitHub Pages

O projeto inclui o workflow `.github/workflows/deploy-pages.yml`. A publicação acontece automaticamente após cada push na branch `main`.

1. Crie um repositório no GitHub.
2. Envie este projeto para a branch `main`.
3. No GitHub, acesse **Settings → Pages**.
4. Em **Build and deployment → Source**, selecione **GitHub Actions**.
5. Abra a aba **Actions** e acompanhe o workflow **Deploy to GitHub Pages**.

Ao concluir, o endereço publicado aparecerá no resumo do workflow e em **Settings → Pages**.

O build utiliza caminhos relativos, portanto funciona tanto em sites de projeto (`usuario.github.io/repositorio`) quanto com domínio personalizado.
