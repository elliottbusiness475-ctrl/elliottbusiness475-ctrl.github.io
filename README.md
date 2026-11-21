# Elliott Capital Management : page d'accueil Discord

Page intermédiaire à mettre dans la bio Facebook. Elle s'ouvre comme une page web classique :
une courte intro animée (environ 3 secondes) met en scène la couverture et le monogramme EC,
puis le bouton apparaît pour rejoindre le serveur Discord.

En ligne : https://elliott-capital-management.pages.dev/

Hébergement gratuit sur Cloudflare Pages, relié à ce dépôt : chaque modification validée ici
est publiée automatiquement en une minute environ. L'ancienne adresse github.io redirige
vers la nouvelle.

## Changer le lien d'invitation Discord

1. Ouvrez `index.html` (bouton crayon « Edit » sur GitHub).
2. Cherchez `nR2uU6tKAw` et remplacez le code par celui de la nouvelle invitation
   (deux endroits : le bouton `href="https://discord.gg/..."` et le champ `value="discord.gg/..."`).
3. Validez avec « Commit changes ». La page est mise à jour en une minute environ.

Utilisez une invitation qui n'expire jamais (Discord : Inviter des gens → Modifier le lien
d'invitation → Expire après : Jamais, Utilisations : Pas de limite).

## Ce que fait la page

- Intro jouée une seule fois par visite ; un toucher la passe ; aucune animation si le téléphone
  est réglé sur « réduire les animations ».
- Bouton vers l'invitation Discord, sans passer par le système de redirection de Facebook
  (le code d'invitation est sensible à la casse : une version en minuscules renvoie « invitation invalide »).
- Dans le navigateur intégré de Facebook, Instagram ou Messenger :
  - sur Android, le bouton ouvre directement l'application Discord, avec repli sur le lien web ;
  - sur iPhone, un bouton propose d'ouvrir la page dans Safari, qui passe la main à l'application Discord ;
  - si le visiteur revient sur la page après avoir touché le bouton, l'aide s'affiche juste en dessous.
- Bouton « Copier » pour coller le lien dans Discord ou dans un autre navigateur.
- Polices et images servies par le site lui-même (aucun appel à des services tiers au chargement).

## Fichiers

- `assets/couverture-*.webp` : la couverture Facebook, en trois tailles.
- `assets/monogramme.webp` : le monogramme EC détouré de la photo de profil.
- `assets/cinzel-latin.woff2`, `assets/jost-latin.woff2` : polices Cinzel et Jost (licence OFL).
