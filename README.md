[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/SkUppgPp)
- Nom: Prin
- Prénom: Max
- URL du site:
- Url de la maquette : https://www.figma.com/design/37uf0I4ss0MS7PWKlBJges/Maquette-SAE-203-Prin-Max?node-id=1201-2&t=Z72ziZMmaKdG4j05-1

# Sujet : Description de la SAE

Cette SAÉ s’inscrit dans le prolongement de la SAÉ 105 du premier semestre...

En partant du travail effectué lors de cette SAE, vous devrez :

- Reprendre les éléments graphiques de l’interface en vue de l’améliorer
- Réaliser la version bureau de l’interface
- Reprendre totalement l’intégration en vue d’une intégration Vite / Vue 3 / Tailwind / Pocketbase
- **Mettre en ligne le site sur votre VPS**

# Consignes

- Le rendu se fait en publiant vos modifications dans ce dépôt.
- Le site doit être publié à une adresse publique sous peine de perdre des points dans toutes les matières.
- Lire les consignes et répondre aux éventuelles questions sur ce même document.
- [ ] Cochez si vous avez compris !

Pour éventuellement archiver ou tester séparément votre projet, **Le rendre en plus sur Moodle** simplement faire une archive de tout le dossier.

## Consignes Intégration (Xavier Senente)

### Maquette

À partir de la maquette réalisée lors de la SAÉ 105, apporter quelques corrections mineures pour améliorer l’interface mobile du site. Réaliser ensuite la version bureau.

Conseil ⇒ mettez en place une grille pour agencer le contenu dans la version bureau.

Exportez les icônes vectorielles au format SVG.

### Intégration

Voici les attendus pour cette partie :

- Structure du code HTML (pertinence sémantique du code HTML + validation)
- Définition des paramètres graphiques dans le fichier tailwind.config.js (couleurs + typo)
- Définition des styles bases
- Définition de quelques classes utilitaires souvent utilisées
- Mise en place du responsive
- Utilisation des grilles avec CSS grid
- Interactions (menu mobile, carrousel, effet de scroll…)

## Consignes Système d'information (Abdallah Makhoul)

Pour la partie backend on vous demande de faire deux collections (architectes, Batiments), même si vous n'utilisez qu'une seule dans la partie Frontend.

Voici les attendus concernant cette partie :

- Un modèle conceptuel de données
- Structuration de la base de données et saisie de données dans Pocketbase
- Saisir les données dans PocketBase
- Un fichier `backend.mjs` comportant les fonctions suivantes qui sont testées dans un fichier `testback.js`
  - une fonction qui retourne la liste de tous les bâtiments
  - une fonction qui retourne la liste de tous les architectes
  - une fonction qui retourne les infos d'un architecte en donnant son id en paramètre avec liste de ses bâtiments
  - une fonction qui retourne la liste des bâtiments d'un architecte donné (par son nom)
  - une fonction qui retourne la liste des bâtiments triés par date de construction (d'une manière chronologique) 
  
- **travail supplémentaire :**
  - **saisir ou modifier des données automatiquement à partir du front**
  - **une page de connexion (en utilisant la collection users)**

Assurez-vous que vous rendez les fichiers suivants (liens) :

- [ ] [backend](/pocketbase/backend.mjs)
- [ ] [test backen](/pocketbase/testback.js)
- [ ] [MCD](/pocketbase/MCD.pdf)

## Consignes Développent web (Pierre Pracht)

Recopier les fonctions de `/pocketbase/backend.mjs` dans le `/src/backend.ts` existant. C'est le premier qui est noté en Système d'information. Le second indirectement dans le cadre de ma matière.

Si vous avez fini la base de données (PocketBase), n'oublier pas de générer ou régénérer `/src/pocketbase-types.ts` . Simplement faire :

```
npm run typegen
```

Réalisez le site en utilisant VueJS/ViteJS fourni et configuré pour l'usage TailwindCSS.

- Usage de `<RouterLink>` et `<RouterView>`
- Pages et routes paramétriques
- Usage de `<Suspense>` et d'"`avait`" pour récupérer les données du backend. (appel de fonction)

Barème indicatif :

- Minimum pour la moyenne :
  - 10 pour un site complet et bien intégré, mais ne faisant qu'une simple boucle pour afficher une collection.
  - Peu descendre jusqu'à 7 si peu ou pas d'intégration.
  - Des points retirés pour tous les problèmes affectant le site ou la qualité du code.
- Pour plus que 10 :
  - 12 afficher la liste d'une collection sur une page et le détail d'un élément de la collection sur une page
  - Jusqu'à 14, si plusieurs pages affichant les données de différentes façons et toujours bien intégrées.
  - Vous pouvez perdre jusqu'à 4 points pour une intégration absente.
  - Jusqu'à +2 points pour l'usage exhaustif de TypeScript.
    - Dont 1 point, si `/src/pocketbase-types.ts` fait et à jour.
  - Jusqu'à +2 points pour l'intégration d'une page 404 bien intégrée.
  - Jusqu'à +2 points pour l'affiche de tailles, couleurs, positions... pilotées par des classes CSS ou styles. (eg. frise.)

## Consignes Hébergement (Hakim Mabed)

L'évaluation se fait exclusivement sur la base des réalisations faites sur le VPS

Barème de l'évaluation Hébergement :
- Accessibilité du backoffice de pocketbase (http://sousdom.dom.tld:xxxx/_/ ou http://adresseip:xxxx) -> **4 pts**
- Connexion au backoffice de pocketbase via l'email et mot de passe fournis -> **2 pts**
- Disponibilité des collections et des users dans le backoffice de pocketbase -> **3 pts**
- Association d'un nom de sous domaine à l'application web (nom-sous-domaine.mon-domaine.tld) -> **2 pts**
- Accessibilité de l'application en http ou https -> **4 pts**
- Inscription d'un nouveau utilisateur par un email, nom et mot de passe -> **3 pts**
- Connexion de l'application aux données de Pocketbase du VPS -> **2 pts**

Barème de l'évaluation Optimisation :
- Accessisibilité de l'application web via l'URL https://sousdom.dom.tld -> **7 pts**
  Sinon accessisibilité de l'application web via l'URL http://sousdom.dom.tld -> **2 pts**
- Optimisation du score SEO de l'application Web en utilisant Lighthouse -> **5 pts**
- Implémentation d'un serveur Web Mutualisé (fichier 000-default.conf à retourner)-> **6 pts**
  
**P.S. si les accès par https sont OK alors l'accès en http n'est plus nécessaire !**

Renseigner les informations suivantes :

- [ ] Donnez l'adresse IP de votre VPS :
      
- [ ] Donnez le numéro de port d'écoute (xxxx) de pocketbase sur le VPS :
      
- [ ] Donnez le login et le mot de passe admin du compte pocketbase sur le VPS :

- [ ] Donnez l'URL du site web relatif à la SAE203 (sousdom.dom.tld) publié sur le VPS:

- [ ] Joindre le contenu du fichier de configuration apache 000-default.conf utilisé sur le VPS  [APACHE](/apache/000-default.conf)
