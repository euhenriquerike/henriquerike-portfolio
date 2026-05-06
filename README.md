# Henrique rike — Portfolio

## Como subir no GitHub Pages

1. Crie um repositório no GitHub (ex: `henriquerike-portfolio`)
2. Coloque o `index.html`, o `avatar.png` e as imagens/vídeos na mesma pasta
3. Faça o push:
   ```
   git init
   git add .
   git commit -m "portfolio"
   git branch -M main
   git remote add origin https://github.com/SEU_USER/henriquerike-portfolio.git
   git push -u origin main
   ```
4. No repositório > Settings > Pages > Source: **Deploy from branch** > branch `main` > pasta `/root` > Save
5. Em alguns minutos o link aparece: `https://SEU_USER.github.io/henriquerike-portfolio`

## Como adicionar conteúdo

### Avatar
- Salve a ilustração como `avatar.png` na mesma pasta do `index.html`

### Vídeos
Dentro de `<!-- VIDEOS -->` no HTML, substitua os `<div class="video-slot">` placeholder:

- **Arquivo local** (.mp4 na pasta):
  ```html
  <div class="video-slot">
    <video controls autoplay muted loop playsinline>
      <source src="video1.mp4" type="video/mp4">
    </video>
  </div>
  ```

- **Instagram** (pegue o link embed: ··· > Incorporar):
  ```html
  <div class="video-slot">
    <iframe src="https://www.instagram.com/p/CODIGO/embed/" scrolling="no" allowtransparency></iframe>
  </div>
  ```

### Designs
Dentro de `<!-- DESIGNS -->`, substitua os placeholders:
```html
<div class="design-item">
  <img src="design1.jpg" alt="Rock in Rio">
</div>
```
