# Héberger les polices vous-même

## Pourquoi

Vos mentions légales annoncent qu'aucune donnée n'est transmise à un tiers.
Tant que la page appelle `fonts.googleapis.com`, c'est faux : à chaque
visite, le navigateur envoie à Google l'adresse IP du visiteur, sa page
d'arrivée et son navigateur, avant même qu'il ait cliqué sur quoi que ce
soit. La CNIL a sanctionné exactement cela. C'est le seul point du site
qui contredit vos propres mentions.

La correction : télécharger les fichiers une fois, les poser à côté de
`index.html`, remplacer trois lignes.

---

## 1. Les fichiers exacts — **huit**

J'ai mesuré ce que la page rend vraiment, graisse par graisse. Il en faut
huit, pas un de plus.

### Libre Baskerville — les titres

| Graisse | Où elle sert |
|---|---|
| **400 normal** | les titres de section, les questions de la FAQ |
| **400 italique** | tous les mots en `<em>` — « plus loin », « sur votre réalité » |
| **700 normal** | trois titres seulement, mais ils sautent aux yeux si le gras est faux |

### Outfit — tout le reste

| Graisse | Où elle sert |
|---|---|
| **300** | le corps de texte, les paragraphes longs |
| **400** | les libellés courants |
| **500** | les surtitres, les étiquettes de couleur, les dates |
| **600** | les boutons secondaires, les onglets |
| **700** | les boutons dorés et les badges |

> Le 700 d'Outfit manquait dans l'appel de la page : le navigateur
> fabriquait un faux gras en épaississant le 400. C'est corrigé dans cette
> version — et c'est une raison de plus de le télécharger pour de bon.

---

## 2. Où les prendre

Ouvrez **https://gwfh.mranftl.com** (google-webfonts-helper) dans votre
navigateur — moi je n'y ai pas accès depuis ici.

**Libre Baskerville**

1. Cherchez `Libre Baskerville`
2. Charsets : cochez **latin** et **latin-ext**
3. Styles : cochez **regular**, **italic**, **700**
4. Bouton *Download files*

**Outfit**

1. Cherchez `Outfit`
2. Charsets : **latin** et **latin-ext**
3. Styles : **300**, **regular**, **500**, **600**, **700**
4. *Download files*

---

## 3. Les renommer

Créez un dossier `fonts/` à côté de `index.html` et rangez-y les huit
fichiers `.woff2` sous **exactement** ces noms — c'est le seul point où
une faute de frappe casse quelque chose :

```
fonts/baskerville-400.woff2
fonts/baskerville-400-italic.woff2
fonts/baskerville-700.woff2
fonts/outfit-300.woff2
fonts/outfit-400.woff2
fonts/outfit-500.woff2
fonts/outfit-600.woff2
fonts/outfit-700.woff2
```

Ignorez les `.woff` (sans le 2) et les `.ttf` : plus lourds, et plus aucun
navigateur en circulation n'en a besoin.

---

## 4. Les trois lignes à remplacer

Dans `index.html` **et** dans `pt.html`, cherchez ce bloc dans le `<head>` :

```html
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Libre+Baskerville:ital,wght@0,400;0,700;1,400&family=Outfit:wght@300;400;500;600;700&display=swap" rel="stylesheet">
```

Supprimez ces trois lignes. À la place, collez ceci :

```html
<style>
  /* polices hébergées ici : rien ne part vers un serveur tiers */
  @font-face{font-family:'Libre Baskerville';font-style:normal;font-weight:400;
    font-display:swap;src:url('fonts/baskerville-400.woff2') format('woff2');}
  @font-face{font-family:'Libre Baskerville';font-style:italic;font-weight:400;
    font-display:swap;src:url('fonts/baskerville-400-italic.woff2') format('woff2');}
  @font-face{font-family:'Libre Baskerville';font-style:normal;font-weight:700;
    font-display:swap;src:url('fonts/baskerville-700.woff2') format('woff2');}
  @font-face{font-family:'Outfit';font-style:normal;font-weight:300;
    font-display:swap;src:url('fonts/outfit-300.woff2') format('woff2');}
  @font-face{font-family:'Outfit';font-style:normal;font-weight:400;
    font-display:swap;src:url('fonts/outfit-400.woff2') format('woff2');}
  @font-face{font-family:'Outfit';font-style:normal;font-weight:500;
    font-display:swap;src:url('fonts/outfit-500.woff2') format('woff2');}
  @font-face{font-family:'Outfit';font-style:normal;font-weight:600;
    font-display:swap;src:url('fonts/outfit-600.woff2') format('woff2');}
  @font-face{font-family:'Outfit';font-style:normal;font-weight:700;
    font-display:swap;src:url('fonts/outfit-700.woff2') format('woff2');}
</style>
```

Le `font-display:swap` fait que le texte s'affiche tout de suite dans une
police système, puis bascule : jamais de page blanche pendant le
chargement.

---

## 5. Vérifier

Une fois en ligne, ouvrez le site, faites un clic droit → *Inspecter* →
onglet **Réseau**, rechargez. Filtrez sur `google` : la liste doit rester
vide. Si elle l'est, vos mentions légales disent vrai.

Et regardez un bouton doré : le gras doit être net, pas boursouflé.
