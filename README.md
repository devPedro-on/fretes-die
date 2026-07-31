# Fretes Die

🔗 **Site no ar:** https://fretes-die.vercel.app

Site de apresentação e conversão de clientes para a **Fretes Die** — fretes e pequenas mudanças na região metropolitana, interior e litoral do RS.

- Instagram: [@fretes_die](https://www.instagram.com/fretes_die/)
- WhatsApp: [(51) 99476-4662](https://wa.me/5551994764662)

## Sobre

Página única (landing page) estática, sem frameworks ou build step: HTML, CSS e JS puros. Feita para carregar rápido e converter visitantes em contatos pelo WhatsApp.

Seções: hero, serviços, galeria de trabalhos realizados, diferenciais e contato, com botão flutuante de WhatsApp fixo.

## Estrutura

```
index.html      página principal
style.css       estilos (tema preto/dourado)
script.js       pequeno script (ano do rodapé)
serve.js        servidor estático simples, usado só para rodar localmente
img/            fotos dos trabalhos + ícones (logo e favicon)
```

## Rodando localmente

Requer [Node.js](https://nodejs.org) instalado.

```bash
node serve.js
```

Depois acesse `http://localhost:8792`.

## Atualizando conteúdo

- **Fotos da galeria**: substitua os arquivos em `img/01.jpg` a `img/10.jpg` (mesmos nomes) ou edite as tags `<img>` na seção `#galeria` do `index.html`.
- **WhatsApp**: o número aparece em vários links no formato `https://wa.me/5551994764662`. Para trocar, use busca e substituição em `index.html`.
- **Textos**: todo o conteúdo (serviços, diferenciais, textos do hero) está direto no `index.html`, sem CMS.

## Deploy

O site está publicado na Vercel como projeto estático (sem build). Qualquer push para a branch `main` no GitHub gera um novo deploy automaticamente.

Para deployar manualmente:

```bash
vercel --prod
```
