# Site do treinamento (acesso pela web)

Página web estática, em português, com todo o material: cronograma, setup,
os 3 módulos com código copiável e checkpoints interativos.

## Acessar localmente

Abra o arquivo `index.html` no navegador, ou sirva a pasta (recomendado):

```bash
cd treinamento-flutter
python3 -m http.server 8080 --directory site
# → http://localhost:8080
```

Servindo a partir da raiz do treinamento, os alunos também baixam/abrem
`projeto-starter/` pela mesma origem.

## Publicar na web (opções)

| Opção | Como |
|---|---|
| **GitHub Pages** | Suba `site/` para um repository → Settings → Pages → publicar da branch |
| **Netlify / Vercel** | Arraste a pasta `site/` (deploy estático, sem build) |
| **Servidor interno / wiki** | Copie `index.html` (arquivo único, CSS/JS embutidos) |

Não há dependências, build nem backend: é um único `index.html`.
