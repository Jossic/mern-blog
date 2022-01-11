---
title: 'Setup un backend NodeJs avec Fastify, Typescript et Jest'
excerpt: 'Setup un backend NodeJs avec Fastify, Typescript et Jest'
coverImage: '/assets/blog/build-fastify-backend/fastify.png'
date: '2022-01-11T09:43:07.322Z'
author:
    name: Jossic Lapierre
    picture: '/assets/blog/authors/jo.png'
ogImage:
    url: '/assets/blog/build-fastify-backend/fastify.png'
---

## Setup un backend NodeJs avec Fastify, Typescript et Jest

Cet article a pour but de centraliser une bonne pratique (selon moi) de construction d'un backend en nodeJs avec Fastify, Typescript et Jest. :joy:

### Technos

---

-   ![NodeJS logo](/assets/blog/build-fastify-backend/nodejs.png)
-   ![Image Fastify](/assets/blog/build-fastify-backend/fastify-logo.png)
-   ![Jest logo](/assets/blog/build-fastify-backend/jest.png)
-   ![Typescript logo](/assets/blog/build-fastify-backend/typescript.png)

### Sources

---

Pour réaliser ce backend, je me suis servi de certaines sources :

-   [https://www.youtube.com/watch?v=WHV57q6p3Lk&ab_channel=JayWolfe](https://www.youtube.com/watch?v=WHV57q6p3Lk&ab_channel=JayWolfe)
-   [https://www.youtube.com/watch?v=beY0sn-XgtY&t=537s&ab_channel=JayWolfe](https://www.youtube.com/watch?v=beY0sn-XgtY&t=537s&ab_channel=JayWolfe)

### Premières étapes

---

![Image Fastify](/assets/blog/build-fastify-backend/fastify-logo.png)

-   On installe le client
    > `yarn global add fastify-cli`
-   On initialise le projet
    > `fastify generate monProjet --lang=ts`
-   On se rend dans le dossier
    > `cd monProjet`
-   Lancement en mode dev
    > `yarn dev`
-   Pour tester
    > `curl localhost:3000`

#### Installation de la config de la vidéo (_Facultatif_)

-   Sur mac, pour télécharger le fichier de config
    > `brew install wget`
-   On télécharge le fichier
    > `wget https://gist.githubusercontent.com/wolfejw86/22a29bd6565fb679959c83c5bc40fea5/raw/9ac1869e4d4d91a41a37d0739b11e1b4de62612f/setup-typescript-eslint-prettier.js`
-   On execute le fichier
    > `node setup-typescript-eslint-prettier.js`
-   On peu également changer le PORT, mis par défaut sur 3000, pour cela, il faut créer un fichier .env dans la racine du projet, et y ajouter:
    > `FASTIFY_PORT=8080`

### Installation de Jest

---

![Jest logo](/assets/blog/build-fastify-backend/jest.png)

-   On installe de dépendances
    > `yarn add jest ts-jest @types/jest -D`
-   On initialise
    > `npx ts-jest config:init`
-   Commande pour lancer
    > `yarn test`
