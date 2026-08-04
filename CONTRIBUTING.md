# Contribuer

Merci de l'intérêt porté au projet ! Les contributions sont les bienvenues, des corrections de fautes aux nouvelles fonctionnalités.

## Développer

Il n'y a rien à installer :

```bash
git clone https://github.com/dsebastien/plan-de-tables-mariage.git
cd plan-de-tables-mariage
xdg-open index.html
```

Modifiez `index.html`, rechargez la page. C'est tout.

> Astuce : l'état est conservé dans le `localStorage`. Pour repartir de zéro pendant vos tests, utilisez le bouton **Réinitialiser**, ou `localStorage.removeItem('plan-de-tables:v1')` dans la console.

## Principes du projet

Ces contraintes sont volontaires — merci de les respecter dans les propositions :

1. **Un seul fichier, aucune étape de build.** `index.html` doit rester ouvrable par double-clic. Pas de bundler, pas de `npm install`, pas de framework.
2. **Aucune donnée ne sort du navigateur.** Pas d'analytics, pas de télémétrie, pas d'appel réseau au-delà du CSS et de la police. Une liste d'invités contient des données personnelles.
3. **Le mobile compte autant que le bureau.** Un plan de table se retouche assis à table, sur un téléphone. Toute interaction en glisser-déposer doit avoir son équivalent « toucher puis toucher ».
4. **Rester simple avant d'être complet.** Une fonctionnalité qui alourdit l'interface pour trois personnes ne vaut probablement pas son coût.

## Style de code

Suivez ce qui existe déjà : JavaScript moderne, sans point-virgule superflu ni conversion de style, indentation à 2 espaces, commentaires et libellés en français. Les classes Tailwind sont utilisées en ligne ; les couleurs partagées passent par les variables CSS de `:root`.

## Signaler un bug

Ouvrez une [issue](https://github.com/dsebastien/plan-de-tables-mariage/issues) en indiquant :

- ce que vous attendiez et ce qui s'est produit ;
- le navigateur et le système ;
- si possible, un export JSON minimal reproduisant le problème — **en remplaçant les vrais noms par des noms fictifs**.

## Proposer un changement

1. Ouvrez une issue avant les gros chantiers, pour éviter le travail perdu.
2. Créez une branche, faites votre modification, testez à la souris **et** au toucher (les outils de développement du navigateur suffisent).
3. Vérifiez qu'un export puis un réimport (plan et liste) fonctionnent toujours.
4. Ouvrez une pull request en décrivant le problème résolu.

## Licence

En contribuant, vous acceptez que votre contribution soit publiée sous [licence MIT](LICENSE).
