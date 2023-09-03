# Le NIPoPow Sur Ergo : Pour L’Adoption Et L’Interopérabilité

Ergo aime particulièrement sortir des chemins battus pour construire la blockchain de demain. Ainsi, une fonctionnalité trop méconnue est le NIPoPoW : Non-Interactive Proof of Proof of Work. Ce nom barbare cache la possibilité d’accroître sensiblement la scalabilité des blockchains en Proof of Work.

Le NIPoPoW fut découvert par l’équipe d’IOHK qui développe la blockchain Cardano et où a travaillé Alexander Chepurnov avant de fonder Ergo.

C’est donc tout naturellement qu’Ergo permet le NIPoPoW depuis sa création.

Malgré un nom compliqué, nous allons voir ensemble en quoi consiste cette innovation puis ce qu’elle pourra apporter aux blockchains.

## Comment fonctionne le NIPoPoW ?
### Un petit rappel du Proof of Work (PoW)
Avant d’aller plus loin, il faut bien comprendre ce qu’est un protocole en Proof of Work (PoW).

Pour fonctionner, une blockchain doit inscrire toutes les transactions dans des blocs. Ces blocs sont créés à une certaine fréquence. Dans un protocole en PoW, des ordinateurs réalisent des calculs afin de résoudre une équation. Le premier qui résout l’équation crée un bloc et obtient une récompense associée. L’intégralité de l’historique des blocs permet de s’assurer qu’il n’y a pas d’éléments malveillants au milieu. Les ordinateurs doivent donc conserver cet historique complet pour s’assurer de la fiabilité du réseau. Et au fur et à mesure de l’évolution de la blockchain, sa taille peut peser plusieurs Gigaoctets.

### Heureusement arrive le PoPoW
Mais le NIPoPoW permet de réduire considérablement la taille de la blockchain à archiver. En effet, le Po juste avant le PoW introduit le Proof of Proof of Work. Schématiquement, on demande une preuve du bon fonctionnement du Proof of Work. Nous n’avons plus besoin de connaître l’intégralité des blocs qui composent une blockchain pour nous assurer de sa fiabilité.

L’équipe d’IOHK a observé un phénomène des plus étranges survenir dans les blockchains en PoW. De temps en temps et de manière aléatoire est créé un bloc particulier appelé superbloc. Ce bloc est beaucoup plus difficile à miner (son équation plus difficile à résoudre) et il comprend un nombre de zéro beaucoup plus important que les autres.

Quand, dans la plupart des blockchains, ces superblocs restent une curiosité ; sur Ergo, on leur attribue un rôle crucial. En effet, dans l’entête de ce superbloc, Ergo y ajoute des données qui archivent l’intégralité des informations contenues dans les blocs présents depuis le superbloc précédent.

Ainsi, vous l’aurez compris, on peut connaître l’historique complet de la blockchain en “lisant” uniquement les superblocs.

Ainsi, on peut résumer une blockchain de plusieurs Gigaoctets en moins de 1 Mo.

### Et le NI alors ?
« NI » pour Non-Interactive. Cela signifie que le système tourne en arrière plan sans nécessité de permission ou de participation au protocole. En gros, n’importe qui peut accéder à la Proof of Proof of Work et c’est totalement gratuit.

Bref, parfait pour développer des applications du quotidien sur des bases solides (même niveau de sécurité que le Proof of Work) et légères (moins de 1 Mo !).

## Que peut permettre le NIPoPoW d’Ergo?
### Des applications légères… et sans tiers de confiance
Ergo est une plateforme de smart contracts qui permet à de nombreuses applications de voir le jour. Dans l’exemple qui suit, nous allons parler des wallets car c’est le plus parlant pour tout le monde, mais on peut extrapoler à toutes les applications actuelles et futures autour de la blockchain.

Avec nos portefeuilles, aujourd’hui, il faut faire un choix.

La première option est d’être maître à 100% de son wallet en utilisant un portefeuille directement rattaché à un nœud du réseau que l’on doit héberger. Mais cela nécessite un matériel puissant et assez de mémoire pour stocker l’intégralité de la blockchain. De plus, à chaque fois que l’on souhaite utiliser son wallet, il faut synchroniser son nœud à la blockchain et cela peut prendre plusieurs minutes voire plusieurs heures.

Devant ces contraintes, beaucoup se tournent vers une autre option : les light wallets. Avec ces derniers, on peut héberger son portefeuille sur un smartphone, l’ouvrir rapidement et réaliser des transactions sans devoir attendre une quelconque synchronisation. La contrepartie à cette praticité est que, pour y arriver, le wallet se connecte à un nœud hébergé par un tiers de confiance. Ainsi, on s’éloigne fortement de la décentralisation. Nos transactions peuvent être soumises à la censure si le tiers de confiance nous refuse l’accès par volonté propre ou sous la pression d’un gouvernement.

Le NIPoPoW permet d’allier le meilleur des deux mondes. Grâce aux superblocs, l’intégralité des données de la blockchain peut peser moins de 1 MB. Un wallet construit autour de cette fonctionnalité pourra être stocké sur un smartphone et se synchroniser en quelques secondes. Ainsi, on se retrouve avec des lights wallets sans devoir passer par un quelconque tiers de confiance.

La fonctionnalité NIPoPoW sur Ergo permettra de construire des applications pratiques et conviviales tout en conservant les fondations décentralisées et permissionless de la blockchain. C’est une condition nécessaire à l’adoption de masse que très peu d’autres blockchains réellement décentralisées peuvent se permettre.

### Et aussi des mineurs “lights”
Les mineurs Bitcoin doivent tous stocker plusieurs centaines de Go d’historique de blockchain. À cause des smart contract, la blockchain Ethereum pèse plus d’1 To. Autant dire qu’il en faut du stockage pour miner !

Si Ergo est amené à devenir une plateforme incontournable pour smart contracts, on parlera aussi d’une blockchain qui pèse des To. Mais quel sera l’ordre de grandeur dans 20 ans ? Ce n’est clairement pas soutenable.

Le NIPoPoW, en permettant de créer des full node hyper légers, permettra à tout un chacun de miner avec un appareil standard. Imaginons que demain les pools de minage soient censurées ou qu’elles décident d’elles-mêmes de censurer une partie de la population ; une masse d’acteurs isolés pourront leur mettre des bâtons dans les roues en minant dans leur coin avec un équipement abordable.

Et ce scénario ne sera possible que grâce au NIPoPoW. Cette fonctionnalité est donc aussi un atout majeur dans la décentralisation du protocole.

### Une révolution dans l’interopérabilité et développement des sidechains
Dernier point, et pas des moindres, le développement des layers 2 et sidechains. La difficulté des sidechains réside dans l’interaction entre les bockchains. Les échanges de coins d’une chaîne à l’autre créent des vulnérabilités qui sont souvent compensées par une centralisation des sidechains.

Le NIPoPoW permet de résoudre ce problème. En effet, il permet d’être considéré comme un certificat et de déclencher des smart contracts ou transactions sur la sidechain en toute sécurité.

Par exemple, 1 Erg envoyé sur une adresse spécifique de burn pourrait très bien déclencher un smart contract sur une autre blockchain.

Un usage spécifique dans la Defi serait de se passer des wrapped tokens qui permettent par exemple d’échanger des Bitcoins sur la plateforme Ethereum. L’utilisation du NIPoPoW permettrait de réaliser cette opération de manière beaucoup plus sûre et totalement décentralisée.

Il y a peu, Vitalik Buterin émettait des doutes sur l’avenir de tous les bridges interblockchains en train d’apparaître, car trop risqués. On ne peut que lui donner raison au vu des derniers gros hacks connus.

Mais ce n’est pas une raison pour abandonner l’idée de sidechains et d’interopérabilité, car le NIPoPoW a le potentiel de résoudre toutes ces difficultés. En effet, cette fonctionnalité permettrait de simplifier et sécuriser les interactions entre blockchains de manière totalement décentralisée.

## Ergo, NIPoPOW et avenir
Comme nous venons de le voir, le NIPoPoW représente une révolution au sein de l’univers blockchain et Ergo a l’insolence de l’intégrer nativement. Quand d’autres blockchains comme Bitcoin, Ethereum Classic (mais pas Ethereum, car en transition vers du POS) devront adapter leur protocole pour l’exploiter pleinement, Ergo est la seule bockchain à pousser dès aujourd’hui les recherches et les essais sur cette nouvelle technologie.

Car oui, le NIPoPoW a été découvert fin 2018 et nous n’en sommes qu’à ses débuts. Les cas d’usage pourront être encore plus incroyables au fur et à mesure des développements au sein de l’écosystème crypto…

Autant de perspectives positives pour Ergo qui sera amener à devenir une blockchain de premier plan.
