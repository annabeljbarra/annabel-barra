# Fiche 2 — Faire vivre le site sur annabel-barra.com

*Une seule séance. Comptez 20 minutes chez Gandi, puis de l'attente.*

## Ce qu'on fait, et pourquoi

Aujourd'hui `annabel-barra.com` **redirige** vers GitHub : le visiteur
tape votre adresse et atterrit sur une autre. On arrête de rediriger et
on fait pointer le domaine **directement** sur le site. Après ça,
`annabel-barra.com` sera la vraie adresse, celle qui s'affiche dans la
barre du navigateur et dans Google.

Pourquoi ça vaut le coup : c'est votre adresse, elle tient sur une carte
de visite, et le jour où vous quittez GitHub vos affiches imprimées
restent valables.

## Avant de commencer

**Le site doit être publié.** Si ce n'est pas fait, faites-le d'abord
(fiche 1) et revenez ici.

---

## Étape 1 — Supprimer la redirection

Chez Gandi, dans votre domaine → **Redirections web**. Supprimez celle
qui existe.

Tant qu'elle est là, elle occupe le domaine et rien d'autre ne peut
fonctionner. C'est aussi ce qui créerait une **boucle infinie** si on
faisait les choses dans l'autre ordre : GitHub renverrait vers
annabel-barra.com, qui renverrait vers GitHub, sans fin.

## Étape 2 — Saisir neuf enregistrements DNS

Toujours chez Gandi, dans votre domaine → **Enregistrements DNS**.
Le nom `@` désigne le domaine nu, sans www.

| Type | Nom | Valeur |
|---|---|---|
| A | `@` | `185.199.108.153` |
| A | `@` | `185.199.109.153` |
| A | `@` | `185.199.110.153` |
| A | `@` | `185.199.111.153` |
| AAAA | `@` | `2606:50c0:8000::153` |
| AAAA | `@` | `2606:50c0:8001::153` |
| AAAA | `@` | `2606:50c0:8002::153` |
| AAAA | `@` | `2606:50c0:8003::153` |
| CNAME | `www` | `annabeljbarra.github.io.` |

Les quatre `A` sont les quatre serveurs de GitHub. Il les faut **tous les
quatre** : c'est ce qui fait que le site tient si l'un d'eux tombe. Les
`AAAA` sont leurs équivalents pour les connexions modernes.

Le **point final** après `annabeljbarra.github.io.` est voulu. Chez Gandi
il signifie « adresse complète, n'ajoute rien derrière ». Sans lui, Gandi
écrirait `annabeljbarra.github.io.annabel-barra.com`, qui n'existe pas.

Laissez le TTL par défaut.

## Étape 3 — Déclarer le domaine côté GitHub

Dépôt `annabel-barra` → **Settings** → **Pages** → **Custom domain**.
Saisissez `annabel-barra.com`, **Save**.

GitHub ajoute tout seul un fichier `CNAME` au dépôt et se met à vérifier
le DNS. Une pastille passe au vert quand c'est bon.

## Étape 4 — Attendre, puis forcer le HTTPS

Comptez de quelques minutes à 24 heures. Revenez ensuite sur la même page
et cochez **Enforce HTTPS**.

Tant que la case est grise, la propagation n'est pas finie : ce n'est pas
une panne, c'est de la patience. C'est cette case qui fera disparaître le
`http://` que Google affiche aujourd'hui.

---

## Comment savoir que ça marche

Tapez `annabel-barra.com` dans une fenêtre de navigation privée. Le site
doit s'afficher **et l'adresse doit rester `annabel-barra.com`** dans la
barre — plus de bascule vers github.io. Avec un cadenas.

Essayez aussi `www.annabel-barra.com` : il doit arriver au même endroit.

## Ce que je fais ensuite

Vos deux pages et le sitemap déclarent encore l'ancienne adresse. Dès que
le domaine répond, dites-le-moi : je réécris les trois fichiers et vous
n'aurez qu'à les remonter.

**Ne déclarez le sitemap dans la Search Console qu'après ça** — envoyé
tel quel, il serait rejeté.
