# PA AUTO — intermédiation en commerce de gros

Site vitrine statique (HTML / CSS / JS, sans build) hébergé sur GitHub Pages,
domaine `paauto.shop`.

> Généré depuis `C:\Users\souha\coaching-sites-factory` (fichier `sites/paauto.mjs`).
> Pour une modification de contenu, éditez ce fichier puis relancez `node build.mjs paauto` :
> une modification faite directement ici serait écrasée à la prochaine génération.

## À compléter avant de communiquer sur le site

| Priorité | Quoi | Où |
|---|---|---|
| 🔴 Bloquant | Mentions légales : identité de l’éditeur, SIREN, adresse, médiateur. Obligatoire en France. | `mentions-legales.html` |
| 🟠 Important | Adresse `contact@paauto.shop` : créer une redirection e-mail chez Namecheap (*Domain List → Manage → Redirect Email*). | Namecheap |
| 🟠 Important | Formulaire : remplacer `VOTRE_ID_FORMSPREE` (sinon repli automatique en `mailto:`). | `contact.html` |
| 🟠 Important | Présentation de la personne qui coache (nom, parcours réel, photo). | `a-propos.html` |
| 🟡 Plus tard | Tarifs (Commission / Commission / Non €) et contenu des formules à ajuster à votre offre réelle. | `index.html` `#tarifs` |
| 🟡 Plus tard | Témoignages : n’en ajoutez que des vrais, avec l’accord des personnes. | — |

## Description de l’activité (Stripe, annuaires…)

```
We are PA AUTO, a wholesale trade intermediary based in Namur, registered since April 2017 under activity code 46.180, agents specialised in the wholesale of particular products. We bring buyers and suppliers together and we assemble the file that a cross-border sale has to stand on. That file is the whole subject, because since January 2020 the exemption on an intra-Community supply of goods no longer depends on formalities. It depends on substantive conditions: the customer must communicate a valid VAT identification number issued by another Member State, and the supplier must file a correct intra-Community sales listing. Fail either and the exemption falls away, and the VAT is the supplier's to pay. Two further points decide the rest. A VAT number has to be checked in the European verification system on a dated and retained basis, because a number valid last month can be deregistered by delivery. And proof of dispatch rests on a presumption that needs at least two non-contradictory documents from two parties independent of both seller and buyer, which is hardest to satisfy when the buyer collects the goods. We claim no trading record. Site: paauto.shop
```

## Structure

```
index.html            Accueil : hero, programmes, méthode, tarifs, approche, FAQ
programmes.html       Détail des 4 programmes
a-propos.html         Notre approche et principes
contact.html          Formulaire de prise de contact
mentions-legales.html Mentions légales, confidentialité, CGV
404.html              Page d’erreur (chemins absolus)
assets/css/style.css  Couleurs de la marque en tête de fichier, puis styles communs
assets/js/main.js     Menu, thème, animations, formulaire
```

## DNS (Namecheap → Advanced DNS)

Supprimer les enregistrements de parking, puis :

| Type | Host | Value |
|---|---|---|
| A Record | `@` | `185.199.108.153` |
| A Record | `@` | `185.199.109.153` |
| A Record | `@` | `185.199.110.153` |
| A Record | `@` | `185.199.111.153` |
| CNAME Record | `www` | `hamzaniceguy99-glitch.github.io.` |
