# À FAIRE — Annabel Barra

*Version du site : **V47**. Mis à jour le 13 septembre 2026.*
*Fusion de ce document et de `A-FAIRE_Annabel_tableau-de-bord.docx`.*

---

# 🔴 URGENT — rien d'autre n'avance tant que ce n'est pas fait

| Tâche | Qui | Durée |
|---|---|---|
| **Publier le site** | vous | 10 min |

**Rien n'est en ligne.** Ce que voient vos visiteurs — et ce que montre
Google — est toujours la première version : titre « Constellations
familiales & coaching », onglet « Entreprises », pas de NIF, pas
d'adresse, pas de médiateur.

1. Ouvrir `site-V47-A-PUBLIER`
2. GitHub, dépôt `annabel-barra` → **Add file** → **Upload files**
3. Glisser le **contenu** du dossier — pas le dossier. `img/` reste un
   sous-dossier.
4. **Commit**
5. **Settings → Pages** : source `main`, dossier `/ (root)`
6. Trois minutes, puis **Cmd + Maj + R**

> Ne touchez pas à « Custom domain » : tant que la redirection Gandi
> existe, ça créerait une boucle. C'est la fiche 2 qui s'en occupe.

Puis, une fois en ligne : **nettoyer le dépôt** — supprimer les anciens
fichiers qui ne sont pas dans les treize du dossier.

---

# 🟠 IMPORTANT — dans les deux semaines

| Tâche | Qui | Fiche |
|---|---|---|
| Le domaine `annabel-barra.com` | vous puis moi | `FICHE-2-DOMAINE-GANDI.md` |
| La fiche Google | vous | `FICHE-3-FICHE-GOOGLE.md` |
| Demander des avis à vos stagiaires | vous | ci-dessous, § Avis |
| Les polices (RGPD) | vous | `POLICES.md` |
| Tests post-publication | vous | ci-dessous, § Tests |

## Le domaine

Google indexe `annabel-barra.com` pendant que vos pages déclarent
`github.io`. La redirection Gandi n'est pas permanente, d'où ce
désaccord. Tout est dans la fiche 2 : supprimer la redirection, saisir
neuf enregistrements DNS, déclarer le domaine côté GitHub, forcer le
HTTPS. Ensuite je réécris les adresses dans les deux pages et le
sitemap.

**Sur vos publications, imprimez toujours `annabel-barra.com`** — jamais
l'adresse en github.io. Elle fonctionne déjà.

## La fiche Google

Elle s'appelle encore « VALUE FOR HUMANS COACHING ». Fiche 3 : la
renommer `Annabel Barra` (rien d'autre — un descriptif après le nom fait
suspendre le profil), les catégories, la description de 743 caractères
prête à copier, la zone desservie, les photos.

**À faire avant de demander des avis**, sinon les nouveaux témoignages
atterrissent sur l'ancien nom.

## Les avis {#avis}

**Le lien** : profil d'établissement → *Demander des avis* → adresse en
`g.page/r/…/review`. Envoyez-la-moi : elle va dans le QR de l'affiche.

**Le moment** : 48 à 72 h après la fin. **Le canal** : WhatsApp,
individuellement.

**Le message portugais**

> Olá [nome],
> Espero que o que se moveu no workshop continue a assentar com calma.
>
> Tenho um pedido, se lhe fizer sentido. Quem procura constelações no
> Algarve não me conhece — lê o que escreveram as pessoas que já
> participaram. Algumas linhas suas sobre o que a trouxe e o que levou
> consigo fariam muita diferença.
>
> É aqui, leva dois minutos: [lien]
>
> E se preferir não escrever, não há problema nenhum. Fico contente na
> mesma por ter estado consigo.
>
> Annabel

**Le message français**

> Bonjour [prénom],
> J'espère que ce qui a bougé pendant l'atelier continue de se déposer
> tranquillement.
>
> Une demande, si ça vous parle. Les personnes qui cherchent des
> constellations ne me connaissent pas — elles lisent ce qu'ont écrit
> celles qui sont déjà venues. Quelques lignes sur ce qui vous a amenée
> et ce que vous en avez rapporté feraient beaucoup.
>
> C'est ici, ça prend deux minutes : [lien]
>
> Et si vous préférez ne pas écrire, aucun souci. Je suis contente de
> vous avoir eue avec moi de toute façon.
>
> Annabel

**Trois interdits.** Aucune contrepartie (réduction, cadeau, tirage au
sort) — interdit par Google et pratique commerciale trompeuse. Pas de
tri des satisfaites (*review gating*) : même message, même lien, pour
tout le monde. N'écrivez pas à leur place.

**L'affiche** : `affiche-avis-QR.png`, sur votre bureau. Le QR porte un
bandeau « LIEN À INSÉRER » — envoyez-moi le lien et je régénère.

## Les polices

`POLICES.md`. Vos mentions annoncent qu'aucune donnée ne part chez un
tiers, alors que chaque visite envoie l'IP du visiteur à Google. Huit
fichiers, trois lignes à remplacer. Une demi-heure.

## Tests, dans l'heure qui suit la mise en ligne {#tests}

- [ ] Les deux pages sur téléphone
- [ ] Envoyer les **deux** formulaires en vrai (contact + boîte à
      outils) et tester le bouton de téléchargement du PDF
- [ ] Coller le lien dans un WhatsApp à vous-même (c'est ainsi qu'on
      voit `partage.jpg`), puis `…/pt.html`
- [ ] Vérifier le quota mensuel Formspree : **deux** formulaires y
      envoient maintenant
- [ ] Vérifier qu'`annabel-barra.com` sert bien la nouvelle version

---

# 🟡 À DÉCIDER — quand vous voulez, mais ça bloque le reste du site

| Décision | Ce qui en dépend |
|---|---|
| L'entreprise devient-elle l'offre principale ? | ordre des offres, numérotation, couleurs, formulaire |
| La ligne sous votre nom | hero, onglet, aperçu partagé, données structurées |
| L'accord de vos six témoins | mise en ligne |
| Instagram `valueforhumans` | cohérence du nom |
| Le régime de TVA | une mention |

## L'ordre des offres

Si **oui** : passe complète — ordre des pastilles, numérotation 01→04,
code couleur, cartes, formulaire, deux langues, et le badge ★ suit.
Si **non** : renfort visuel léger, dix minutes.
À savoir : le code couleur est accroché à la **position**, pas à
l'offre. Un déplacement sans reprise complète rendrait l'entreprise
corail et le parcours violet.

## La ligne sous votre nom

- **A** — Coaching · Facilitation · Ingénierie de formation
  *Régulier, « catalogue ». Perd le nomadisme.*
- **B** — Nomad coach · Facilitatrice & formatrice
  *Chaleureux, garde « Nomad ». Perd le mot « ingénierie ».*
- **C** — celle d'aujourd'hui. Bancale, mais porte le mot-clé exact.

C'est la même décision que l'ordre des offres, posée deux fois.

## L'accord de vos six témoins

Jean-Baptiste Billaud, Elsa Gailhac, Estelle Genovardo, Brice Bragato,
Chloé Bories, Aline Mendonça figurent nommément, avec fonction et
employeur. Un témoignage nominatif est une donnée personnelle :
**avez-vous leur accord écrit ?** Kizeo est votre premier client
formation — c'est peut-être délicat avant la signature.

## Instagram

Votre compte s'appelle `valueforhumans` et sort dans Google juste sous
votre site. Troisième surface à traiter si le nom doit vraiment
disparaître. Changer l'identifiant est gratuit ; les anciens liens
cessent de fonctionner.

## La TVA

Si franchise en base : **« TVA non applicable — article 293 B du CGI »**
sur les factures, et utile sur le site puisque des prix sont affichés.
Confirmez-moi le régime et je l'ajoute — une mention fausse est pire
qu'absente.

---

# 🟢 SANS URGENCE — des semaines, sans conséquence

## Marque & documents professionnels

| Tâche | Détails | Statut |
|---|---|---|
| Signature mail | colibri · nom, titre, tél, e-mail, site, LinkedIn | à faire |
| Carte de visite | recto/verso, prête à imprimer | à faire |
| Tête de lettre A4 | en-tête + pied de page | à faire |
| Devis type | SIRET/NIF, régime TVA, IBAN, RC pro, **médiateur ✅** | débloqué |
| Facture type | mêmes mentions que le devis | débloqué |

> Le devis et la facture attendaient les coordonnées du médiateur.
> Elles sont désormais connues : **CM2C, 49 rue de Ponthieu, 75008
> Paris, cm2c.net**. Adhésion valable jusqu'au 10/09/2029.

## LinkedIn

| Tâche | Statut |
|---|---|
| Choisir le titre (3 options, A recommandée) | à décider |
| Réécrire « À propos » — même esprit B2B | à faire |
| Photo & bannière — actuelles très bien | OK |

## Le site, finitions

- [ ] **Face FR de la carte** — l'aperçu de la boîte à outils montre la
      face portugaise sur les deux pages. Envoyez-la-moi.
- [ ] **Image pour le bloc Formations** — aujourd'hui mis en avant par
      la couleur seule.
- [ ] **Search Console** — déclarer `sitemap.xml`, **après** ma
      réécriture des adresses.

## Divers

- [ ] **Retitrer les docs stratégie** — choisir le titre à propager
      (marque constellations vs Nomad coach).
- [ ] **Ménage sur le bureau** — une cinquantaine de dossiers de site,
      avec des doublons (`site-V33-A-PUBLIER 2`, `_1`…). Le seul à jour
      est `site-V47-A-PUBLIER`. Ouvrir un autre, c'est voir une vieille
      version et croire qu'une correction a sauté. C'est arrivé deux
      fois.

---

# 📋 Quand le NDA arrivera

La formulation actuelle — *« en cours d'enregistrement auprès de la
DREETS PACA »* — est exacte et n'engage rien.

Au numéro, **la forme est imposée** :

- Conventions, devis, factures : *« déclaration d'activité enregistrée
  sous le numéro … auprès du préfet de région Provence-Alpes-Côte
  d'Azur »*
- Si vous l'affichez sur le site (facultatif) : *« Enregistré sous le
  numéro … Cet enregistrement ne vaut pas agrément de l'État. »*

La seconde phrase n'est pas décorative : article L.6352-12 du Code du
travail.

---

# ✅ Ce que portent les mentions aujourd'hui

Nom · statut · siège (945 Chemin des Crottes, Hameau, Beaumes-de-Venise)
· SIRET · NIF portugais · `annabeljbarra@gmail.com` · téléphone ·
directrice de la publication · hébergeur complet · RGPD complet
(responsable, finalités, durée de conservation, droits, CNIL et CNPD) ·
absence de cookies · nature non médicale des accompagnements ·
**médiateur de la consommation CM2C**.

**Plus rien ne manque.**

**Non obligatoires chez vous** : pas de CGV exigées (aucun paiement sur
le site), pas de RCS (vous n'êtes pas commerçante), pas de déclaration
d'accessibilité (réservée aux organismes publics et aux grandes
entreprises).

**Un point resté ouvert** : CM2C couvre votre activité française. Le
Portugal a ses propres entités de résolution alternative de litiges, et
la loi portugaise demande d'informer le consommateur de l'entité
compétente. La page portugaise le précise (« atividade em França »).
À creuser un jour, sans urgence.

*Je ne suis pas juriste : sur la TVA et sur le volet portugais, un avis
professionnel vaut mieux que le mien.*
