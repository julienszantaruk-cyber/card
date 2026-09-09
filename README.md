# Julien Grimond-Szantaruk — digital business card

## English

1. **Add the photo:** place a file named `photo.jpg` beside `index.html`. The card will show the `JGS` initials automatically if the image is missing.
2. **Edit the bio:** open `index.html`, find `<!-- BIO -->` inside `<section id="about">`, and insert your text immediately before or after that comment.
3. **Publish with GitHub Pages (free):**
   - Create a public repository, for example `card`.
   - Upload `index.html`, `contact.vcf`, `qr.html`, `qr.png`, `qr.svg`, `README.md`, and optionally `photo.jpg`.
   - In **Settings → Pages**, choose **Deploy from a branch**, select `main` and `/ (root)`, then save.
   - Your card will be at `https://USERNAME.github.io/card/`. Replace `USERNAME` with the real account name.
4. **Alternatives:** drag the folder into [Netlify Drop](https://app.netlify.com/drop), or import the repository into [Vercel](https://vercel.com/). Both can host these static files for free on their standard plans.
5. **Regenerate the QR:** after the final URL is known, run this one-line command from the folder (requires Python and `qrcode`):
   `python -c "import qrcode; qrcode.make('https://REAL-URL.example/').save('qr.png')"`
   To update the printable SVG too, use the `qrcode` package's SVG factory or regenerate it with a short Python script. Update the URL text and note in `qr.html` as well.

## Français

1. **Ajouter la photo :** placez un fichier nommé `photo.jpg` à côté de `index.html`. Si l'image manque, la carte affiche automatiquement les initiales `JGS`.
2. **Modifier la bio :** ouvrez `index.html`, repérez `<!-- BIO -->` dans `<section id="about">`, puis insérez votre texte autour de ce commentaire.
3. **Publier gratuitement avec GitHub Pages :** créez un dépôt public (par exemple `card`), téléversez les fichiers, puis allez dans **Settings → Pages**. Choisissez **Deploy from a branch**, la branche `main` et le dossier racine `/`. L'adresse sera `https://USERNAME.github.io/card/`.
4. **Alternatives :** déposez le dossier dans [Netlify Drop](https://app.netlify.com/drop), ou importez le dépôt dans [Vercel](https://vercel.com/).
5. **Régénérer le QR :** quand l'URL définitive est connue, exécutez :
   `python -c "import qrcode; qrcode.make('https://VOTRE-URL.example/').save('qr.png')"`
   Mettez également à jour l'URL affichée dans `qr.html`.
