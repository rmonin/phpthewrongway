# Utilise toujours un _framework_ #

> Tous les _frameworks_ PHP non spécifique puent!
>
> -- [Rasmus Lerdorf](https://www.youtube.com/watch?v=DuB6UjEsY_Y)

Dans la communauté PHP une très mauvaise tendance est devenue la norme de facto pour le développement d'applications Web; l'utilisation d'un _framework_ populaire non spécifique.

Cette tendance a émergée et est devenue populaire non pas parce qu'elle améliore le résultat du processus de développement, ou parce que c'est la bonne chose à faire en partant d'une technologie et d'un point de vue architectural. Cette tendance est devenue populaire parce que certains développeurs de _frameworks_ ont réussi à influer sur les masses avec leur polémique contre la programmation native avec des phrases comme "Ne Réinvente pas la roue !" et "Ne le fait pas toi-même, d'autres sont plus doués que toi".

Beaucoup de programmeurs d'aujourd'hui ignorent complètement les principes fondamentaux de la programmation et ils passent une grande partie de leur temps à fantasmer sur de nouvelles couches de complexité pour paraître plus intelligent, plus cool, et acceptés par tous ceux qu'ils considèrent comme leurs pairs.

Ces personnes semblent être obsédés par l'idée d'avoir d'autres personnes qui suivent leur «façon de faire», devenant une sorte de leader PHP de la communauté, et ayant d'autres personnes utilisant leurs derniers outils hmodernes" _Open Source_, qu'ils en oublient de faire en sorte que les conseils qu'ils donnent soient sains et robustes.

Dans l'industrie du logiciel, vous pouvez comparer une maison pré-construite à un _framework_ non spécifique. Construire des logiciels utilisant des _frameworks_ non spécifique ne fait pas de vous plus un codeur ou un programmeur mais quelqu'un qui assemble une maison pré-construite, vous êtes un charpentier.

Sur ce site, nous distinguons entre les _frameworks_ et les bibliothèques de la façon suivante :

* Une bibliothèque est considérée comme une collection de code réutilisable, comme la bibliothèque standard C, ou la bibliothèque standard Go. Il se compose de code que vous intégrez facilement dans vos propres projets sans appliquer des limitations ou restrictions que ce soit. Il se compose de petits morceaux de code avec chacun une fonctionnalité spécifique.
* Un _framework_ n'est pas seulement une collection de code réutilisable : vous ne pouvez pas simplement prendre un morceau de code de _framework_ et l'intégrer dans votre propre projet. Un _framework_ est un système qui vous aide à construire un logiciel, mais en même temps, il vous oblige à travailler dans les limites et les restrictions du _framework_ lui-même. Un _framework_ a beaucoup de fonctionnalités interdépendantes. Un morceau ne peut pas fonctionner sans l'autre.

Dans le monde de Python et Ruby, contruire un site de zero est fatigant, parce que ni Python, ni Ruby a été initialement créé pour construire des sites Web. Par conséquent de manière générale des _frameworks_ tels que [Django](https://fr.wikipedia.org/wiki/Django_%28framework%29) et [Ruby on Rails](https://fr.wikipedia.org/wiki/Ruby_on_Rails) sont rapidement devenus populaire pour construire des sites dans ces langues.

PHP d'autre part a été créée au début par Rasmus Lerdorf comme un ensemble d'outils écrits en C qui vous permettront de développer facilement et rapidement de l'HTML dynamique. En tant que tel PHP était, et est toujours, ** un _framework_ en soi **.

PHP has evolved massively since then and today PHP can be used for much more than building HTML and websites, but viewing PHP as a sort of framework in itself is not wrong. PHP is by nature a layer of abstraction for developing web applications written entirely in a procedural C.

Using a library within your project is only natural. PHP itself comes bundled with a set of libraries that you can use to extend your own code. PDO for example is a lightweight library that provides a consistent interface for accessing databases in PHP.

Using a framework on top of PHP on the other hand is another matter entirely.

When you use a framework in PHP you add a layer of abstraction on top of yet another layer of abstraction, one that was already in place for you to use to begin with. The added layer of abstraction that the framework provides may simply serve to organize your code into a pre-fixed set of patterns, or it may add even more complexity by intertwining hundreds or even thousands of classes and methods into a nightmare of dependencies, either way you're adding layers of complexity to your code that isn't needed!

All experience starts with the interface. The interface experience is the result of the underlying technology and the amount of layers of abstraction. The more abstraction you use, the less efficient the interface becomes and the more error-prone the application becomes. The higher the abstraction, the more detail and efficiency is lost.

Understand this clearly: **The ideal number of lines of code in any project is as few as possible whilst being as clear and readable as possible!**

> What everyone doesn't need is a general purpose framework. Nobody has a general problem, everyone has a very specific problem they are trying to solve.
>
> -- [Rasmus Lerdorf](https://www.youtube.com/watch?v=anr7DQnMMs0)

Some companies began listening to the hype about PHP frameworks and they started their next projects using one of these popular general purpose frameworks only to end up in a disaster. Not only did they discover that the general purpose framework was really bad at solving their very specific need, but it was also extremely slow in doing so. It was impossible to scale and as a result they started ripping the framework apart in a desperate attempt to pull out all those things they really didn't need.

Always use the pragmatic approach:

> Action or policy dictated by consideration of the immediate practical consequences rather than by theory or dogma.
>
> -- Collins English Dictionary, Complete and Unabridged, 12th Edition 2014

**The wrong way:** Always use a framework on top of PHP. ![Thumbs down](/img/thumbs-down.png)
