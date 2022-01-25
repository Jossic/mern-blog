---
title: 'Setup un front React Native, Typescript et Jest'
excerpt: 'Setup un front React Native, Typescript et Jest'
coverImage: '/assets/blog/build-react-native-typescript-jest/reactnative.png'
date: '2022-01-11T09:43:07.322Z'
author:
    name: Jossic Lapierre
    picture: '/assets/blog/authors/jo.png'
ogImage:
    url: '/assets/blog/build-react-native-typescript-jest/reactnative.png'
---

# Setup un front React Native, Typescript et Jest

Cet article a pour but de centraliser une bonne pratique (selon moi) de construction d'un backend en nodeJs avec Fastify, Typescript et Jest. :joy:

## Technos

---

-   ![Expo logo](/assets/blog/build-react-native-typescript-jest/expo-logo.png)
-   ![React Native logo](/assets/blog/build-react-native-typescript-jest/react-native.png)
-   ![Typescript logo](/assets/blog/build-fastify-backend/typescript.png)
-   ![Jest logo](/assets/blog/build-fastify-backend/jest.png)
-   ![Tailwind CSS logo](/assets/blog/build-react-native-typescript-jest/tailwindcss.png)

## Sources

---

Pour réaliser ce backend, je me suis servi de certaines sources :

-   [https://www.typescriptlang.org/](https://www.typescriptlang.org/)

## Premières étapes

---

-   On installe le client expo
    > `yarn global add explo-cli`
-   On initialise le projet
    > `expo init mon-projet` > ![Expo init](/assets/blog/build-react-native-typescript-jest/expo-init.png)
-   On se rend dans le dossier > `cd mon-projet`

    ## Setup tailwind

---

    ### Sources

    -   [https://www.npmjs.com/package/tailwind-react-native-classnames](https://www.npmjs.com/package/tailwind-react-native-classnames)

-   [https://www.npmjs.com/package/tailwind-rn](https://www.npmjs.com/package/tailwind-rn)

-   Deux solutions Tailwind React Native Classnames | tailwind-rn
    > `expo install tailwind-react-native-classnames`

## Installation de Jest - react testing library

---

![Jest logo](/assets/blog/build-fastify-backend/jest.png)

-   On installe de dépendances
    > `yarn add jest ts-jest @types/jest @testing-library/react-native jest-expo -D`
-   On initialise
    > `npx ts-jest config:init`
-   Commande pour lancer

    > `yarn test`

    ## Setup ESlint + prettier

---

    ### Sources

-   [https://edusutil.medium.com/eslint-with-prettier-settings-for-react-native-ce13d2aaf500](https://edusutil.medium.com/eslint-with-prettier-settings-for-react-native-ce13d2aaf500)
-   [https://github.com/vasilestefirta/react-native-eslint-prettier-example](https://github.com/vasilestefirta/react-native-eslint-prettier-example)

-   On initialise

    > `npx eslint --init`

    ## Setup AWS Amplify

---

    ### Sources
