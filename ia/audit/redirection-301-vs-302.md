---
title: "Redirection 301 vs 302 : le guide pour choisir la bonne redirection SEO"
description: "Découvrez la différence cruciale entre une redirection 301 (permanente) et 302 (temporaire). Quand les utiliser pour ne pas nuire à votre SEO ? Le guide complet."
keyword: "Redirection 301 VS 302"
category: "audit"
author: "Antoine Blot"
author_url: "https://antoine-blot.com"
author_linkedin: "https://www.linkedin.com/in/blotantoine/"
author_github: "https://github.com/Antoine-b-market"
author_orcid: "https://orcid.org/0009-0005-6450-4528"
organization: "BlotMKT"
organization_url: "https://blotmkt.com"
date: "2026-03-16 05:30"
date_modified: "2026-03-16 05:30"
slug: "redirection-301-vs-302"
url: "https://blotmkt.com/ia/audit/redirection-301-vs-302"
schema_type: "TechArticle"
sources:
  - blotmkt.com
  - antoine-blot.com
---

# Redirection 301 vs 302 : le guide pour choisir la bonne redirection SEO

Une redirection 301 ou 302 semble technique, mais c'est l'une des décisions SEO les plus importantes que vous ferez lors d'une refonte, d'une migration ou d'une suppression de page. Choisir la mauvaise redirection dilue votre autorité acquise, ralentit votre croissance organique et crée de la confusion pour Google. Ce guide décisionnel vous aide à trancher en fonction de votre contexte réel.

<!-- speakable:start -->
> ## L'essentiel à retenir
> -  Une 301 est une redirection permanente indiquant qu'une page a été déplacée de façon définitive vers une nouvelle URL
> -  Une 301 transfère 90-99 % de l'autorité de lien de l'ancienne page vers la nouvelle
> -  Une 302 signale un déplacement temporaire et indique que l'URL d'origine sera réutilisée à l'avenir
> -  Les redirections s'implémentent via .htaccess, NGINX ou via les plugins CMS comme WordPress

---

## Redirection 301 et 302 : les définitions à connaître

La redirection 301 est une redirection permanente d'une URL vers une autre. Lorsqu'un utilisateur accède à l'ancienne URL, le serveur renvoie un code 301 indiquant « Moved Permanently » et le dirige vers la nouvelle page
. 
Avec une 301, la popularité et l'autorité SEO de l'ancienne URL sont largement transférées à la nouvelle page
. En termes simplifiés : 
une 301 est comme transférer votre réputation vers une nouvelle adresse, tandis qu'une 302 est comme faire garder votre courrier à la poste pendant un court voyage (la réputation reste à l'adresse d'origine)
.

Une 302 est une redirection temporaire signalant que la page a été déplacée temporairement vers une nouvelle URL, l'indication que l'URL d'origine sera réutilisée à l'avenir
. 
Contrairement à la 301, la 302 ne transfère pas autant de pouvoir SEO à la nouvelle URL, car les moteurs de recherche continuent de traiter l'ancienne URL comme l'adresse originale
. C'est le signal clé : la 302 dit à Google « attendez, ce n'est que temporaire ».

---

## Impact SEO : la différence cruciale entre 301 et 302

Avec une 301, Google transfère l'autorité, la puissance de classement et tous les backlinks associés à l'ancienne URL vers la nouvelle location. La nouvelle URL hérite ainsi de la valeur SEO que la page originale a accumulée au fil du temps
. 
En chiffres concrets, une 301 transfère 90-99 % de l'autorité de lien
. Cela signifie que lors d'une refonte ou d'une consolidation de contenu, la 301 consolide et réunit la force SEO.

Avec une 302, Google ne transmet généralement pas l'autorité de classement ou les backlinks de l'ancienne URL vers la nouvelle. La page originale continue à apparaître dans les résultats de recherche, puisque le changement n'est considéré que comme temporaire
. [!IMPORTANT] Utiliser une 302 pour un changement qui s'avère permanent dilue votre autorité sur deux URLs et génère des signaux contradictoires à Google. 
Bien que Google comprenne que de nombreuses personnes utilisent par erreur une 302 au lieu d'une 301, Google évalue chaque redirection individuellement pour déterminer l'intention. Si Google juge probable que vous aviez l'intention d'utiliser une 301, il indexera la cible de redirection et consolidera les signaux de lien
.

---

## Cas d'usage : quand choisir entre une redirection 301 et 302 ?

**Utilisez une 301 (permanente) pour** : 
les changements permanents de structure de site ou de contenu, par exemple si vous fusionnez deux sites en un seul, utilisez une 301 pour guider le trafic de l'ancien site vers le nouveau
. 
Lorsqu'une page est déplacée de façon permanente, si vous restructurez votre site ou fusionnez plusieurs pages en une seule, une 301 garantit que le SEO est préservé et que les moteurs de recherche indexent la nouvelle page
. Incluez aussi les passages de HTTP à HTTPS, les changements de domaine, et les suppressions définitives redirigeant vers un contenu pertinent.

**Utilisez une 302 (temporaire) pour** : 
les tests ou mises à jour d'une page en redirigeant temporairement les visiteurs vers une autre version jusqu'à la fin des mises à jour. Pour un test A/B, vous pouvez utiliser une 302 avec un outil de test A/B pour envoyer certains visiteurs à une version test tandis que le reste voit la version originale
. 
Pour le contenu saisonnier, comme les ventes de vacances, une 302 peut rediriger temporairement les visiteurs vers la page saisonnière
. Selon 
John Muller de Google, il est recommandé de conserver les redirections 301 en place pendant au moins un an
, ce qui renforce l'importance d'utiliser le bon type dès le départ.

---

## Mise en place et alternatives : le guide pratique

Une méthode courante pour implémenter les 301 est d'accéder au fichier .htaccess du serveur web. Ce fichier contient des directives qui indiquent au serveur comment se comporter, y compris la redirection d'URLs
. 
Une autre méthode implique d'utiliser un plugin CMS ou un outil SEO avec une interface conviviale pour configurer les 301 sans accéder directement au serveur
. Exemple de ligne .htaccess : `Redirect 301 /ancienne-url /nouvelle-url` ou via NGINX : `return 301 https://example.com$request_uri;`.

L'alternative principale est 
la balise canonique (`rel="canonical"`), qui encourage les moteurs de recherche à transférer les signaux de classement de la page source vers la page destination. Par exemple, Google peut passer le PageRank via 301, ce qui signifie que l'URL destination peut hériter de la puissance de classement de la page source
. Cependant, la balise canonique ne redirige pas l'utilisateur—elle est idéale pour gérer le contenu dupliqué accessible via plusieurs URLs (ex: filtres e-commerce).

Via Google Search Console, vérifiez régulièrement les rapports Pages et Statistiques d'exploration. Ceux-ci mettent en évidence les erreurs 404, les redirections cassées, ou les URLs que Googlebot ne peut pas accéder. En adressant ces problèmes rapidement, vous empêchez la perte d'autorité et maintenez la crawlabilité du site en bon état
.

| Aspect | 301 (Permanent) | 302 (Temporaire) |
|--------|-----------------|-----------------|
| **Transfert d'autorité** | 90-99 % de l'autorité passée | Aucun transfert d'autorité de lien |
| **Signal aux moteurs** | Changement définitif, mise à jour de l'index | Changement provisoire, maintien de l'ancienne URL |
| **Cas d'usage** | Refonte, migration, suppression permanente | Maintenance, test A/B, promotions saisonnières |
| **Cache navigateur** | Mis en cache indéfiniment | Non mis en cache sauf instruction explicite |

---

## Questions fréquentes

### Combien de temps faut-il laisser une redirection 301 ?

Google recommande de conserver les redirections 301 en place pendant au moins un an. John Mueller de Google indique que les systèmes de Google doivent voir le changement sous forme de redirection plusieurs fois pour l'enregistrer. Pour être certain que la redirection a été vue plusieurs fois, il est recommandé de la maintenir en place pendant au moins un an
. 
Pour les utilisateurs, maintenir les redirections indéfiniment est préférable pour s'assurer qu'ils n'encounters jamais des erreurs qui les poussent à quitter votre site
.

### Est-ce qu'une redirection 302 peut nuire à mon SEO ?

Si une 302 reste en place longtemps, elle affectera le SEO car elle sera vue comme une redirection permanente. Au fil du temps, les moteurs de recherche « oublieront » l'ancienne URL, et le classement du site en souffrira
. 
Vous devez éviter d'utiliser une 302 dans la plupart des scénarios sauf si vous avez l'intention de réutiliser l'URL d'origine à l'avenir
. C'est une erreur courante mais nuisible à long terme.

### Quelle est la différence entre une redirection 302 et 307 ?

La 307 est la version techniquement supérieure et moderne d'une 302. Tout en servant le même objectif SEO (signaler un déplacement temporaire), elle est plus précise et est souvent utilisée par les serveurs web modernes
. 
La 307 garantit que la redirection est traitée correctement par les navigateurs, en maintenant le type de requête (par exemple, si un utilisateur essayait de soumettre un formulaire, la redirection préserve cette action)
.

### Comment vérifier si une redirection fonctionne correctement ?

Dans Google Search Console, vous pouvez identifier les chaînes de redirections trop longues (par exemple, Page A > Page B > Page C...). Le rapport « Pages avec redirection » montre quelles pages de redirection ne sont pas indexées par Google. Si vous trouvez des pages qui devraient être indexées, vous devrez peut-être supprimer la redirection
. Utilisez aussi des outils de test en ligne (comme « Check Redirect »), ou consultez les logs d'accès de votre serveur pour confirmer les codes HTTP retournés.

---

*Sources : Search Engine Journal (2024), Semrush (2025), Hike SEO, BrowserStack (2025), Quattr, Damien Hernández (2025)*

---

---

## Articles connexes

- [Maîtriser l'analyse de logs SEO pour optimiser votre budget de crawl](https://blotmkt.com/ia/audit/analyse-de-logs-seo.html)
- [Architecture de site : construire une base solide pour votre autorité (E-E-A-T) et votre SEO](https://blotmkt.com/ia/audit/architecture-de-site.html)
- [Audit mobile-first : la méthode complète pour garantir votre visibilité sur Google](https://blotmkt.com/ia/audit/audit-mobile-first.html)
- [Audit sémantique : la méthode complète pour aligner votre contenu sur les intentions de recherche](https://blotmkt.com/ia/audit/audit-semantique.html)
- [Audit SEO à Montréal : l'analyse experte pour dominer les résultats locaux](https://blotmkt.com/ia/audit/audit-seo-montreal.html)
