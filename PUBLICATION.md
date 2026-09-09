# Mise en ligne — V38

Ce dossier **est** le site. Tout ce qu'il contient va à la racine du dépôt
GitHub, en gardant la structure : le sous-dossier `img/` reste un
sous-dossier.

```
index.html          la page française
pt.html             la page portugaise
img/                les cinq images du site
boite-a-outils.pdf  le document des 5 questions
partage.jpg         l'image qui s'affiche quand on colle le lien (FR)
partage-pt.jpg      la même, portugaise
sitemap.xml         la liste des pages pour Google
robots.txt          l'autorisation d'indexer + où trouver le sitemap
.nojekyll           empêche GitHub de « traiter » les fichiers au passage
POLICES.md          la dernière étape RGPD, à faire après
```

**900 Ko en tout**, contre 1,4 Mo en V29. Les images sont des fichiers
séparés : elles sont mises en cache, et quelqu'un qui passe du français
au portugais ne les retélécharge pas.

> Glissez le **contenu** du dossier, pas le dossier lui-même — sinon le
> site part vivre dans un sous-répertoire. `.nojekyll` est invisible dans
> le Finder : Cmd + Maj + point l'affiche. Il ne sert à rien ici, ne vous
> battez pas avec.

Puis **Settings → Pages** : source `main`, dossier `/ (root)`. Deux à
trois minutes, puis rechargez avec **Cmd + Maj + R** — votre navigateur
a l'ancienne version en cache.

---

# ⚠️ À FAIRE — par ordre d'urgence

## 1. Le médiateur de la consommation

**C'est le seul point qui expose à une amende : 3 000 €.**

Depuis 2016, tout professionnel qui vend une prestation à un particulier
en France doit adhérer à un dispositif de médiation de la consommation
et l'afficher. Il n'y a ni seuil de chiffre d'affaires, ni exonération
pour les auto-entrepreneurs. Le déclencheur est la vente à un
particulier — donc votre premier accompagnement individuel, pas votre
première mission en entreprise.

Ce n'est pas une histoire de litige ni de faute : c'est une obligation
d'**accès au recours**. Vous adhérez, vous affichez le nom, et vous n'en
entendez plus parler — sauf si un jour quelqu'un fait appel à lui.

**Où trouver la liste officielle**

- La liste qui fait foi, tenue par la CECMC au ministère de l'Économie :
  `economie.gouv.fr/mediation-conso` → « Médiateurs référencés »
- L'annuaire ouvert, plus commode à filtrer :
  `data.economie.gouv.fr` → « Annuaire des médiateurs de la consommation »

Le coaching et l'accompagnement n'ont pas de médiateur sectoriel dédié :
cherchez un organisme **généraliste**, référencé pour les prestations de
services aux particuliers. Filtrez sur « services » / « tous secteurs ».

**Attention** : il ne suffit pas d'écrire un nom sur le site. Il faut
d'abord signer une convention avec l'organisme ou accepter ses
conditions. Une mention sans adhésion réelle ne vaut rien.

Comptez quelques dizaines d'euros par an, plus un forfait par médiation
si le cas se présente. Vingt minutes de démarche, une fois.

→ **Envoyez-moi ensuite le nom, l'adresse, le site et l'e-mail du
médiateur.** Je pose le bloc dans les mentions, avec le lien vers la
plateforme européenne de règlement des litiges, dans les deux langues.

## 2. La TVA

Si vous êtes en franchise en base, la mention **« TVA non applicable —
article 293 B du CGI »** doit figurer sur vos factures, et elle est utile
sur le site puisque des prix y sont affichés. Je ne l'ai pas écrite : je
ne connais pas votre régime, et une mention de TVA fausse est pire
qu'absente. Confirmez-moi et je l'ajoute.

## 3. Les polices

Voir `POLICES.md`. C'est le seul point du site qui contredit vos propres
mentions légales : elles annoncent qu'aucune donnée n'est transmise à un
tiers, alors que chaque visite envoie l'IP du visiteur à Google. Huit
fichiers à télécharger, trois lignes à remplacer. Une demi-heure.

## 4. Quand le NDA arrivera

La formulation actuelle du site — *« en cours d'enregistrement auprès de
la DREETS PACA »* — est exacte et n'engage rien.

Quand vous aurez le numéro, **la forme est imposée** :

- Sur vos conventions, devis et factures :
  *« déclaration d'activité enregistrée sous le numéro … auprès du préfet
  de région Provence-Alpes-Côte d'Azur »*
- Si vous l'affichez aussi sur le site — c'est facultatif — la mention
  devient obligatoirement :
  *« Enregistré sous le numéro … Cet enregistrement ne vaut pas agrément
  de l'État. »*

La seconde phrase n'est pas décorative : elle est imposée par l'article
L.6352-12 du Code du travail.

---

# Dans l'heure qui suit la mise en ligne

- [ ] Ouvrir les deux pages sur téléphone, pas seulement sur ordinateur.
- [ ] Envoyer le formulaire de contact **et** celui de la boîte à outils
      pour de vrai : c'est le seul test qui vaille, Formspree ne répond
      qu'à un domaine confirmé. Vérifier que les deux arrivent, et que le
      bouton de téléchargement du PDF fonctionne.
- [ ] Vérifier que la nouvelle adresse `annabel-barra@gmail.com` est bien
      relevée, ou redirigée vers votre boîte principale. Une adresse
      publique que personne ne lit est pire que pas d'adresse.
- [ ] Coller le lien dans une conversation WhatsApp avec vous-même :
      c'est ainsi qu'on voit `partage.jpg`. Puis le lien `…/pt.html`.
- [ ] Vérifier le quota mensuel de votre formule Formspree : **deux**
      formulaires y envoient maintenant, pas un.

# Sans urgence

- [ ] **Google Search Console** — y déclarer `sitemap.xml` accélère
      nettement la première indexation.
- [ ] **La photo d'atelier** est un fichier de 1024 px affiché sur toute
      la largeur : agrandie de 40 % sur grand écran, ça se voit un peu.
      Si vous retrouvez l'original, je la remplace.
- [ ] **L'aperçu de la boîte à outils** montre la face portugaise de
      votre carte, sur les deux pages. Envoyez-moi la face française et
      je fais afficher la bonne selon la langue.

---

# Ce que portent les mentions aujourd'hui

✅ Nom · statut · **siège (Beaumes-de-Venise)** · SIRET · NIF portugais ·
e-mail · téléphone · directrice de la publication · hébergeur complet
(dénomination et adresse) · RGPD complet (responsable, finalités, durée
de conservation, droits, CNIL et CNPD) · absence de cookies · nature non
médicale des accompagnements.

❌ Médiateur de la consommation — voir point 1.

**Non obligatoires chez vous** : pas de CGV exigées (aucun paiement sur
le site), pas de RCS (vous n'êtes pas commerçante), pas de déclaration
d'accessibilité (réservée aux organismes publics et aux grandes
entreprises).

*Je ne suis pas juriste : sur le médiateur et la TVA, un avis
professionnel vaut mieux que le mien.*
