## 1. La méthode sumRange devrait retourner la somme des entiers compris entre 10 et 100 inclusifs contenus dans le tableau passé en paramètre.

```java
 int sumRange(int[] ints) {
    int sum = 0;
      for (int i = 0; i < ints.length; i++) {
        int n = ints[i];
          if (n>=10 || n<=100) {
          sum +=n;
        }
      }
    return sum;
  }
```

## 2. Transformez la méthode Counter.increment() pour qu’elle supporte l’accès concurrentiel de plusieurs threads

## 3. En base 2 (binaire), combien font 0001 & 0001 ?

0001 & 0001 = 1

## 4. Le Garbage collector garanti qu’il y a suffisamment de mémoire pour exécuter un programme java ?

## 5. Implémentez la méthode Algorithm.findLargest(int[] numbers) afin qu’elle retourne le plus grand nombre dans numbers.

```java
  int findLargest(int[] numbers) {
      int max = numbers[0];
      for (int number : numbers) {
        if(number > max) {
          max = number;
        }
      }
      return max;
    }
  }
```

## 6. Parmi ces deux procédures de développement, laquelle préconisez-vous ?

- Procédure #2

  1. Implémenter la nouvelle fonctionnalité “F”
  2. Ecrire des testes pour “F”
  3. Tester que “F” fonctionne correctement

## 7. Que se passe-t-il lors d’un merge “fast-forward” ?

## 8. Quelle commande permet d’effacer la branche distante nommée “branfix” ?

```sh
git push origin --delete remoteBranchName
```

## 9. Un dépôt distant à pour URL https//github.com/exp/hello.git

Ecrivez la commande utilisée pour créer une copie locale de ce dépôt dans le répertoire
courant

```sh
git clone https//github.com/exp/hello.git .
```

## 10. La commande permet de récupérer les nouvelles données d’un dépôt distant sans pour autant combiner ces données avec les fichiers de votre espace de travail ?

```sh
git fetch
```

## Quelle fonctionnalité de Github met à disposition une interface web conviviale pour notifier les membres d’une équipe projet de la fin d’un développement et permet ensuite que les changements proposés soient revus puis intégrés dans la branche master ?

Github Pull request

## Quel est l’usage typique de la commande git bisect ?

Utilisez la recherche binaire pour trouver le commit qui a introduit un bogue

## Quelle commande utilisant l’option — mount permet de monter un volume en lecture seule (dans docker) ?

```sh
docker run -d --mount source=/path/to/src-vol,destination=/path/to/dist-vol,readonly image-name:latest
```

## Pour investiguer un problème, vous avez besoin de lister les ports publiés par un container.

Quelle commande pourriez-vous utiliser dans cette situation ?

```sh
docker inspect --format='{{range $p, $conf := .NetworkSettings.Ports}} {{$p}} -> {{(index $conf 0).HostPort}} {{end}}' $INSTANCE_ID
```

## Y-a-t-il des différences entre les instructions CMD et ENRYPOINT d’un dockerfile ?

- CMD: can override it from docker-client
- ENTRYPOINT: can't override it

## Quelle commande permet de créer un container avec pour un serveur DNS personnalisé 8.8.8.8 ?

## Quel est le rôle de l’instruction EXPOSE dans un Dockerfile ?

## Scrum a-t-il un rôle appelé “Project Manager”

## Quelles différences entre @RequestParam et @PathVariable ?

## Observez les deux façons d’injecter un service dans un bean:

## Quelle annotation peut-on utiliser pour injecter un bean Spring?
