---
layout: page
title: Contribuer
permalink: /contribuer/
---

Les contributions se font à travers le dépôt [GitHub][rust-fr-github]. Vous
pouvez demander des modifications ou les apporter par vous-même si vous
maitrisez les outils adéquates.

# Demander des modifications

Pour demander des modifications, il vous suffit
d'[ajouter un ticket][rust-fr-ticket] sur le dépôt. Vous devrez créer un compte
si vous n'en avez pas, puis décrire avec le plus de détails possible toutes les
modifications que vous souhaitez apporter.

Si vous souhaitez apporter de nombreuses modifications, ou si les différentes
modifications n'ont pas de liens entres elles, il est recommandé de créer
plusieurs tickets, ce qui permet de discuter indépendamment de chaque
modification en cas de besoin.

Après cela, une autre personne prendra en charge le fait d'apporter les
modifications si ces dernières sont acceptées.

# Apporter des modifications

Apporter les modifications vous-même est plus complexe puisqu'il vous faudra
maîtriser tous les outils adéquats.

Forkez le dépôt. Allez sur le [dépôt GitHub][rust-fr-github],
cliquez sur le bouton Fork (vous devez être connecté), puis clonez votre
fork.

    git clone https://github.com/<votre-pseudo>/rust-fr.github.io
    cd rust-fr.github.io

Créez une branche pour vos modifications:

    git checkout -b contrib master

Faites vos modifications, commitez les, puis poussez les sur votre dépôt:

    git commit -a
    git push origin contrib

Créez une pull request. Allez sur la page de votre fork, un bouton `Compare &
pull request` devrait désormais être présent. Cliquez dessus, entrez la
description de vos modifications puis validez.

Une fois la pull request mergée sur le dépôt officiel, vous pourrez aussi
supprimer votre branche si vous le souhaitez :

    git branch -d contrib
    git push origin --delete contrib

Notez qu'il est conseillé de donner un nom à votre branche qui corresponde aux
modifications que vous allez apporter afin de pouvoir la retrouver facilement
si vous faites plusieurs pull requests. Par exemple: `ajout-tuto-lifetime`,
`suppr-lien-invalide`


[rust-fr-github]: https://github.com/rust-fr/rust-fr.github.io "Dépôt GitHub Rust-FR"
[rust-fr-ticket]: https://github.com/rust-fr/rust-fr.github.io/issues/new "Dépôt GitHub Rust-FR - Ajouter un ticket"
[rust-install]: https://www.rust-lang.org/install.html "Installer rust (en)"