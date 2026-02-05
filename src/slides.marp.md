---
marp: true
title: IA, apprentissage et posture humaine
theme: uncover
paginate: true
footer: "_Les liens de l'IA avec les sciences sociales_ - IEP-UPEC - 2026"
style: |
  @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700;800&family=Source+Sans+3:wght@300;400;600;700&display=swap');
  
  @keyframes spotlight1 {
    0% {
      transform: translate(0%, 0%);
    }
    15% {
      transform: translate(30%, 40%);
    }
    30% {
      transform: translate(-20%, 60%);
    }
    45% {
      transform: translate(50%, -10%);
    }
    60% {
      transform: translate(-30%, -20%);
    }
    75% {
      transform: translate(40%, 30%);
    }
    90% {
      transform: translate(-10%, 50%);
    }
    100% {
      transform: translate(0%, 0%);
    }
  }
  
  @keyframes spotlight2 {
    0% {
      transform: translate(-50%, -40%);
    }
    20% {
      transform: translate(45%, -30%);
    }
    40% {
      transform: translate(-35%, 10%);
    }
    60% {
      transform: translate(40%, 45%);
    }
    80% {
      transform: translate(-25%, 55%);
    }
    100% {
      transform: translate(-50%, -40%);
    }
  }
  
  @keyframes spotlight3 {
    0% {
      transform: translate(55%, 45%);
    }
    17% {
      transform: translate(-45%, 35%);
    }
    34% {
      transform: translate(35%, -50%);
    }
    51% {
      transform: translate(-30%, -35%);
    }
    68% {
      transform: translate(50%, 20%);
    }
    85% {
      transform: translate(-40%, -10%);
    }
    100% {
      transform: translate(55%, 45%);
    }
  }
  
  section {
    background: linear-gradient(135deg, #070a1b 0%, #0e0e19 100%);
    background-image: 
      repeating-linear-gradient(0deg, transparent, transparent 2px, rgba(255,255,255,.025) 2px, rgba(255,255,255,.025) 4px),
      repeating-linear-gradient(90deg, transparent, transparent 2px, rgba(255,255,255,.025) 2px, rgba(255,255,255,.025) 4px),
      radial-gradient(circle at 20% 50%, rgba(255,255,255,0.02) 0%, transparent 50%),
      radial-gradient(circle at 80% 20%, rgba(255,255,255,0.015) 0%, transparent 50%),
      radial-gradient(circle at 40% 80%, rgba(255,255,255,0.018) 0%, transparent 50%),
      linear-gradient(135deg, #0a0e27 0%, #1a1a2e 100%);
    position: relative;
    color: #f8f9fa;
    font-family: 'Source Sans 3', sans-serif;
    font-size: 28px;
    padding: 80px;
    justify-content: center;
    overflow: hidden;
    box-shadow: inset 0 0 200px 50px rgba(0, 0, 0, 0.6);
  }
  
  section::before {
    content: '';
    position: absolute;
    top: 50%;
    left: 50%;
    width: 700px;
    height: 700px;
    margin-left: -350px;
    margin-top: -350px;
    background: radial-gradient(circle, rgba(255, 138, 76, 0.18) 0%, rgba(255, 99, 71, 0.1) 30%, transparent 70%);
    animation: spotlight1 56s ease-in-out infinite;
    pointer-events: none;
    z-index: 0;
  }
  
  section::after {
    content: '';
    position: absolute;
    top: 50%;
    left: 50%;
    width: 650px;
    height: 650px;
    margin-left: -325px;
    margin-top: -325px;
    background: 
      radial-gradient(circle at 50% 50%, rgba(138, 255, 195, 0.15) 0%, rgba(76, 255, 178, 0.08) 30%, transparent 70%),
      radial-gradient(circle at 50% 50%, rgba(148, 163, 255, 0.16) 0%, rgba(99, 120, 255, 0.09) 30%, transparent 70%);
    animation: spotlight2 44s ease-in-out infinite, spotlight3 70s ease-in-out infinite;
    pointer-events: none;
    z-index: 0;
  }
  
  section > h1,
  section > h2,
  section > h3,
  section > p,
  section > ul,
  section > ol,
  section > blockquote {
    position: relative;
    z-index: 1;
  }
  
  h1 {
    font-family: 'Poppins', sans-serif;
    font-weight: 800;
    font-size: 2.2em;
    line-height: 1.15;
    margin-bottom: 0.5em;
    text-shadow: 0 4px 20px rgba(0,0,0,0.3);
    letter-spacing: -0.01em;
  }
  
  h2 {
    font-family: 'Poppins', sans-serif;
    font-weight: 600;
    font-size: 1.4em;
    line-height: 1.4;
    margin-top: 0.8em;
    opacity: 0.95;
    letter-spacing: 0em;
  }
  
  h3 {
    font-family: 'Poppins', sans-serif;
    font-weight: 600;
    font-size: 1.15em;
    opacity: 0.9;
    margin-top: 1em;
  }
  
  strong {
    color: #ffc107;
    font-weight: 700;
    text-shadow: 0 2px 10px rgba(255,193,7,0.4);
  }
  
  em {
    color: #82e0ff;
    font-style: italic;
    font-weight: 400;
  }
  
  blockquote {
    border-left: 8px solid #ffc107;
    padding-left: 24px;
    margin: 32px 0;
    font-size: 1.3em;
    font-weight: 300;
    font-style: italic;
    color: #ffffff;
    background: rgba(255,255,255,0.08);
    padding: 16px 24px;
    border-radius: 8px;
  }
  
  ul, ol {
    font-size: 1em;
    line-height: 1.7;
    margin: 30px 0;
  }
  
  li {
    margin: 15px 0;
    padding-left: 10px;
  }
  
  li::marker {
    color: #ffc107;
    font-weight: bold;
  }
  
  footer {
    font-size: 0.6em;
    opacity: 0.7;
    font-weight: 300;
  }
  
  section.lead {
    background: linear-gradient(135deg, #000000 0%, #1a1a2e 50%, #16213e 100%);
    background-image: 
      repeating-linear-gradient(0deg, transparent, transparent 2px, rgba(255,255,255,.025) 2px, rgba(255,255,255,.025) 4px),
      repeating-linear-gradient(90deg, transparent, transparent 2px, rgba(255,255,255,.025) 2px, rgba(255,255,255,.025) 4px),
      radial-gradient(circle at 20% 50%, rgba(255,255,255,0.02) 0%, transparent 50%),
      radial-gradient(circle at 80% 20%, rgba(255,255,255,0.015) 0%, transparent 50%),
      radial-gradient(circle at 40% 80%, rgba(255,255,255,0.018) 0%, transparent 50%),
      linear-gradient(135deg, #000000 0%, #1a1a2e 50%, #16213e 100%);
    text-align: center;
    justify-content: center;
    box-shadow: inset 0 0 200px 50px rgba(0, 0, 0, 0.6);
  }
  
  section.lead h1 {
    font-size: 2.8em;
    margin-bottom: 0.3em;
  }
  
  section.lead h2 {
    font-size: 1.6em;
    font-weight: 400;
    opacity: 0.9;
  }
  
  section.question {
    background: linear-gradient(135deg, #1a0a0e 0%, #4a0e1f 100%);
    font-size: 1.1em;
  }
  
  section.question h1 {
    font-size: 2em;
    text-align: center;
  }
  
  section.concept {
    background: linear-gradient(135deg, #0a1f1a 0%, #0f2f28 100%);
  }
  
  section.alert {
    background: linear-gradient(135deg, #1f0f05 0%, #3d1a08 100%);
  }
  
  section.positive {
    background: linear-gradient(135deg, #0a1a1f 0%, #0f2f3a 100%);
  }
  
  code {
    background: rgba(0,0,0,0.3);
    padding: 4px 12px;
    border-radius: 6px;
    font-family: 'Fira Code', monospace;
  }
  
  a {
    color: #ffc107;
    text-decoration: none;
    border-bottom: 2px solid rgba(255,193,7,0.4);
    transition: all 0.3s ease;
  }
  
  a:hover {
    border-bottom-color: #ffc107;
  }
  
  section::after {
    font-weight: 600;
    text-shadow: 0 2px 8px rgba(0,0,0,0.3);
  }

---

<!-- _paginate: skip -->
<!-- _header: "" -->
<!-- _footer: "" -->
<!-- _class: lead -->

# IA, sciences sociales & apprentissage
> Apprendre mieux, pas seulement plus vite

Pierre-Yves PAMART

<!-- speaker notes
(ENTRÉE CALME – LAISSER UN SILENCE)
Bonjour à toutes et à tous. Aujourd’hui, je ne vais pas vous parler de technologie pour elle-même, mais de vous. De nous. De ce que l’intelligence artificielle dit de notre manière d’apprendre, de progresser, et même de penser.

TRANSITION : Pour démarrer, j’aimerais vous poser une question simple… mais qui n’a rien de technique.
-->

---

## Si l’IA peut faire des choses *à votre place*  
## lesquelles resteront **vraiment les vôtres** ?


<!-- speaker notes
(PAUSE VISUELLE DE 5 SECONDES)

Cette question n’est pas technologique. Elle est humaine. Elle vous invite à réfléchir à ce que vous considérez comme *vraiment vôtre* : votre mémoire, vos idées, vos jugements, vos émotions ?

TRANSITION : Reformulons cette question d’une manière un peu plus directe.
-->

---

## Une autre façon de la poser la question :

### Quand vous utilisez l’IA
### devenez-vous **plus rapides** ou **meilleurs** ?

<!-- speaker notes
C’est toute la tension de cette conférence. Est-ce que l’IA vous aide à aller plus vite — ou est-ce qu’elle vous aide à grandir ? Entre vitesse et valeur, entre performance et compréhension.

TRANSITION : Avant d’aller plus loin, posons le cadre ensemble.
-->

---

# Mettons-nous d’accord

## Cette conférence est interactive

- Interrompez-moi
- Questionnez-moi
- Réfléchissons ensemble

<!-- speaker notes
C’est un échange. Je ne suis pas là pour délivrer un cours magistral, mais pour vous inviter à penser avec moi. Et ce que je dis aujourd’hui, vous avez le droit de le questionner. C’est même recommandé.

TRANSITION : Pour que vous sachiez si je sais ce dont je parle, laissez-moi me présenter en deux mots.
-->

---

# Pierre-Yves PAMART, _PhD_

- Distinguished Engineer dans une banque systémique française
- Directeur de l'expertise
- Mission : **maintenir l’excellence dans le temps**
- Utilisateur quotidien d'outils avec IA

<!-- speaker notes
Je travaille dans un environnement à haute contrainte, à haute performance, avec une attention forte à la responsabilité et à la résilience. J'utilise des outils IA au quotidien, pas pour remplacer, mais pour renforcer la réflexion de mes équipes.

TRANSITION : Et c’est justement ça la nuance. L’IA ne fait pas “à la place de”. Elle change le terrain de jeu — et ça commence dès notre métier.
-->

---

<!-- _footer: "" -->

#### Le software engineering **ce n’est pas que coder**

C'est une discipline de l'**ingénierie**

* Comprendre et explorer les besoins réels
* Parler un langage ubiquitaire
* Modéliser, Architecturer, Implémenter
* Arbitrer
* Supporter
* Assumer les responsabilités
* ... _et encore beaucoup d'autres compétences, savoirs-faire, savoirs-être, faire-savoirs et des responsabilités_

<!-- speaker notes
Ce que j’essaie de transmettre aux jeunes ingénieurs : écrire du code, c’est une petite partie du travail. Le reste, c’est penser des systèmes, gérer la complexité, comprendre le besoin derrière la demande.

Et ça, l’IA ne le fait pas à notre place. Elle génère, elle n’arbitre pas. Elle exécute, elle ne comprend pas.

TRANSITION : Et pourtant, elle est là. Et elle est en train de redéfinir notre quotidien.
-->

___

# L’IA peut écrire du code, 
# mais aussi impacte toutes les autres activités

## L'IA est ou sera *omniprésente*

<!-- speaker notes
Ce n’est plus une tendance. C’est une infrastructure. Elle s’infiltre dans la rédaction, dans la génération d’images, dans l’analyse de données, dans la gestion de projet... jusqu’au recrutement.

L’IA ne reste pas à sa place : elle élargit sans cesse son périmètre.

TRANSITION : Ce changement d’échelle a des conséquences concrètes sur notre environnement de travail.
-->

--- 

# L’IA change l’environnement

* Plus vite  
* Moins cher  
* Plus de pression
* Démultiplie le bon comme le mauvais

<!-- speaker notes
L’IA est un accélérateur. Elle pousse à la performance, à l’instantanéité. Mais elle pousse aussi parfois à l’impatience, à la baisse d’exigence. Et elle rend les erreurs plus rapides, plus visibles, plus graves.

TRANSITION : Et dans ce contexte, une chose ne change pas.
-->

---

# Toutefois

## L'IA ne porte pas la responsabilité.
## L'IA ne vit pas avec les conséquences.

# Vous, **oui**.

<!-- speaker notes
Cette phrase est clé. Elle est même structurante pour la suite de la présentation.  
L’IA ne signe pas. Elle ne répond pas devant le client, devant la direction, devant la société. Elle n’est pas comptable de vos choix.

Vous, oui.

TRANSITION : Alors je vous propose un petit moment d’introspection collective.
-->

---

# Situons-nous un instant

* Qui utilise déjà l’IA ?
* Tous les jours ?
* Pour comprendre ?
* ou seulement pour produire ?

<!-- speaker notes
(LEVER LES MAINS, POSER LES QUESTIONS À VOIX HAUTE)

Je vous propose une auto-évaluation sincère. Pas de bonne ou mauvaise réponse.  
Ce n’est pas ce que vous utilisez qui m’intéresse — c’est comment vous l’utilisez.

TRANSITION : Cette question, on va la rendre visible, en comparant deux postures mentales.
-->

---

# Votre posture

## Humain **augmenté** vs Humain **amélioré** ?

<!-- speaker notes
Je vais ici volontairement exagérer deux postures très différentes pour bien les faire ressortir.  
Ne vous sentez pas enfermés dans l’une ou l’autre. Ce sont deux extrêmes utiles pour penser.

TRANSITION : Voici d’abord ce qu’on appelle l’humain augmenté.
-->

---

# L’humain augmenté

* L’IA fait à la place
* L’IA compense
* Efficacité court terme
* Délégation cognitive
* ## Le but c'est le **livrable** que vous produisez

<!-- speaker notes
L’humain augmenté délègue ses fonctions mentales à la machine.  
C’est pratique. C’est efficace. Mais c’est aussi une forme de renoncement.  
Il livre plus vite, mais apprend moins. Il produit… mais ne progresse pas.

TRANSITION : À l’opposé, voici l’humain qu’on pourrait appeler “amélioré”.
-->

---

# L’humain amélioré

* L’IA entraîne
* L’IA questionne
* Progression long terme
* Capital cognitif
* ## Le but n’est pas le livrable, **c’est ce que vous devenez.**

<!-- speaker notes
L’humain amélioré n’utilise pas l’IA pour aller plus vite.  
Il l’utilise pour aller plus loin.

Il se sert de l’IA comme d’un miroir, comme d’un coach, comme d’un partenaire de questionnement.  
Son objectif : se renforcer lui-même, pas se simplifier.

TRANSITION : Ces deux postures ont des effets bien au-delà de l’individu. Elles touchent la société.
-->

---

# Ce n’est pas neutre socialement

## L’IA accélère les inégalités

<!-- speaker notes
On pense souvent que l’IA pourrait corriger les inégalités.  
Mais en réalité, elle les **accélère**.

Ce n’est pas entre ceux qui ont accès à l’IA et ceux qui ne l’ont pas.  
C’est entre ceux qui l’utilisent pour s’améliorer… et ceux qui l’utilisent pour s’en dispenser.

**Référence :** cette idée rejoint les observations du MIT (2023) et d’Harvard sur l’effet cumulatif de l’usage actif vs passif de l’IA .

TRANSITION : Et cela nous conduit vers un mot que personne n’aime entendre...
-->

---

# Le mot qui dérange

## Atrophie cognitive

<!-- speaker notes
C’est un phénomène simple : ce qu’on n’exerce plus, on le perd.

Des chercheurs du **MIT Media Lab (2023)** ont montré que les personnes utilisant des IA de façon passive activaient **moins de régions cérébrales** liées à la mémoire et à la compréhension .  
Et en plus, elles **retenaient moins bien** ce qu’elles avaient produit avec l’IA.

Donc si vous ne mobilisez plus votre mémoire, votre raisonnement, votre esprit critique… il y a **affaiblissement**.  

Ce n’est pas un effondrement immédiat, c’est une lente glissade.

TRANSITION : Mais il y a une bonne nouvelle dans tout ça.
-->

---

# Bonne nouvelle !

## Votre cerveau peut apprendre toute votre vie

<!-- speaker notes
C’est le principe de la **plasticité cérébrale** : le cerveau se reconfigure à tout âge.  
Des IRM ont montré que de nouveaux circuits se forment même chez des adultes de 60 ans qui apprennent une langue ou un instrument .

Mais pour cela, il faut une chose : **de l’effort**.  
Sans stimulation, sans défi cognitif, il ne se passe rien.

TRANSITION : C’est important, car vous allez bientôt — ou venez juste de — sortir d’école.
-->

---

# Une vérité qui peut déranger

> En sortant de l’école,  
on ne sait pas grand-chose

<!-- speaker notes
Et c’est normal.

On a des bases, quelques repères, parfois de bonnes intuitions.  
Mais les compétences profondes, la pensée critique, la gestion de l’ambiguïté…  
Tout cela s’acquiert **dans la durée**.

Et l’IA ne changera rien à ça. Elle peut vous aider à monter plus vite…  
mais elle ne fait pas le chemin **à votre place**.

TRANSITION : Justement, comment ce chemin se construit-il dans le cerveau ?
-->

---

# Comment le cerveau apprend

## Les quatre piliers

1. Attention  
2. Engagement actif  
3. Feedback et erreur  
4. Consolidation  

<!-- speaker notes
Ces piliers sont issus des travaux de **Stanislas Dehaene** (Collège de France) et validés par des décennies de recherche en psychologie cognitive .

Ils décrivent **ce que le cerveau a besoin** pour apprendre durablement.

TRANSITION : Et on va les explorer un par un, très simplement.
-->

---

# L’attention

## Une ressource limitée

> On n’apprend que ce à quoi on prête attention.

* Filtre d’entrée du cerveau
* Sans attention → pas d’encodage
* Fragile : multitâche, distractions, surcharge cognitive la détruisent
* 👉 Implication pratique : objectifs clairs, rythme, pauses, suppression des distractions.

<!-- speaker notes
C’est le **filtre** de notre cerveau.  
Si vous ne prêtez pas attention à quelque chose, il ne sera **pas encodé** en mémoire.

Or l’IA est une usine à distraction : elle génère du contenu, propose des résumés, fait des raccourcis.  
Mais si vous consommez tout cela **sans prêter attention**, vous ne retiendrez rien.

**Conclusion :** attention fragmentée = apprentissage fragmenté.

TRANSITION : Et ça nous amène au deuxième pilier : il faut être actif, pas passif.
-->

---

# L’engagement actif

## Un cerveau passif n’apprend pas

> On apprend en faisant, pas en regardant.

* Le cerveau doit agir, prédire, manipuler, tester
* L’apprentissage passif (écouter, lire sans effort) est très peu efficace
* 👉 Implication pratique : questions, exercices, expliquer à quelqu’un, résoudre des problèmes.


<!-- speaker notes
Lire ou écouter ne suffit pas. Le cerveau apprend quand il **agit** :  
quand il résout un problème, fait un effort, prédit, se trompe, ajuste.

C’est ce qu’on appelle l’**effort cognitif utile**.

**Exemple simple :** un étudiant qui résout un exercice de tête apprend plus que celui qui regarde juste la correction.

Et une IA peut justement être utilisée… pour créer des problèmes intéressants, des contre-exemples, des dilemmes. Elle peut nourrir l’effort, si vous le cherchez.

TRANSITION : Et pour que cet effort serve vraiment à quelque chose, il faut un bon feedback.
-->

---

# Le feedback et l’erreur

## L’erreur n’est pas un bug c’est une fonctionnalité

> L’erreur est un signal, pas un échec.

* Le cerveau apprend en comparant prédiction vs réalité
* Sans feedback, il ne sait pas ce qu’il doit corriger
* 👉 Implication pratique : feedback rapide, précis, non punitif.
* 👉 Point clé : se tromper est indispensable pour apprendre.

<!-- speaker notes
Le cerveau apprend en **corrigeant ses prédictions**. C’est un mécanisme d’ajustement par l’erreur.

Si on supprime l’erreur, on supprime **la possibilité de progrès**.

**Référence :** les travaux de Dehaene (2015) le montrent bien : quand un enfant réussit du premier coup sans difficulté, il apprend peu. C’est quand il se trompe légèrement puis ajuste qu’il apprend le plus durablement.

Donc quand l’IA vous “protège” de l’erreur, elle vous prive peut-être de l’occasion d’apprendre.

TRANSITION : Encore faut-il que ces apprentissages soient consolidés.
-->

---

# La consolidation

## Comprendre n’est pas maîtriser

> On apprend surtout après avoir appris.

- L’apprentissage se stabilise avec le temps
- Le sommeil joue un rôle central
- La répétition espacée est bien plus efficace que le bachotage
- 👉 Implication pratique : révisions espacées, sommeil suffisant, retour régulier sur les notions.

<!-- speaker notes
On croit souvent que le moment de l’apprentissage, c’est *pendant* le cours ou *pendant* l’exercice.

Mais en réalité, l’apprentissage profond arrive **après**, pendant le sommeil, la relecture, la reformulation.

Mais quelle chose intéressante qu'est finalement la partie bibliographique d'une thèse de doctorat !

**Référence :** études sur la consolidation en mémoire par Robert Bjork (UCLA), qui montrent l’effet bénéfique de l’espacement et du “retrieval practice”.

Le cerveau a besoin de **temps et répétition espacée** pour solidifier.

TRANSITION : Résumons ces 4 piliers par des questions simples.
-->

---

# 🧩 En résumé ultra-synthétique

| Pilier            | Question clé                                         |
|-------------------|------------------------------------------------------|
| Attention         | Suis-je pleinement concentré ?                       |
| Engagement actif  | Est-ce que je fais quelque chose avec l’info ?       |
| Feedback          | Est-ce que je sais si je me trompe ?                 |
| Consolidation     | Est-ce que je laisse le temps au cerveau de fixer ?  |

<!-- speaker notes
Vous pouvez garder cette grille comme outil de vérification.  
À chaque apprentissage, posez-vous ces 4 questions.

Si la réponse est “non” à l’une d’elles… il y a un risque de rétention faible.

TRANSITION : On va maintenant voir quelques **méthodes concrètes** qui exploitent bien ces piliers.
-->

---

# Quelles méthodes d’apprentissages efficaces ?

<!-- speaker notes
Il existe des dizaines de méthodes. Mais toutes les plus efficaces **activent les 4 piliers** que nous avons vus.

Je vais vous en présenter deux principales :  
1. Le **rappel actif** (retrieval practice),  
2. La **pratique délibérée**.

TRANSITION : On commence par la plus puissante et la plus sous-utilisée : la pratique délibérée.
-->

---

# La pratique délibérée

### Comment naissent les experts

> On ne progresse pas en répétant, mais en pratiquant **intentionnellement**, avec effort cognitif, feedback et correction.

* Un objectif clair et spécifique
* Une tâche légèrement au-dessus du niveau actuel
* Un feedback rapide et informatif
* Répétition consciente et ajustée

<!-- speaker notes
Cette méthode a été documentée par le chercheur **Anders Ericsson**, notamment dans son étude sur les violonistes du conservatoire de Berlin (1993).

Les meilleurs étudiants n’avaient pas plus de talent inné, mais **plus d’heures de pratique délibérée**, avec feedback, objectifs clairs, etc.

C’est l’opposé de la répétition automatique.

TRANSITION : Et les musiciens en sont l’exemple vivant.
-->

<!-- speaker notes
Les musiciens sont l’exemple parfait.

Ils ne pratiquent pas plus.
Ils pratiquent mieux.

Pilier 1 — Un objectif clair et spécifique
Description
La pratique délibérée repose sur des objectifs précis, ciblant un aspect identifiable de la compétence.
Pas : « s’entraîner au piano »
Mais : « améliorer la fluidité de la main gauche dans ce passage précis à 80 BPM »
Rôle cognitif
Oriente l’attention
Réduit la charge cognitive
Permet une évaluation objective du progrès
Conséquence pédagogique
Sans objectif précis, l’effort est dissipé → faible progression.

Pilier 2 — Une tâche légèrement au-dessus du niveau actuel
Description
La tâche doit se situer dans une zone de difficulté optimale :
Assez difficile pour provoquer des erreurs
Pas trop difficile pour éviter le découragement
Rôle cognitif
Active la plasticité neuronale
Forçe la réorganisation des schémas mentaux existants
Conséquence pédagogique
Trop facile → automatisation stérile
Trop difficile → surcharge et abandon

Pilier 3 — Un feedback rapide et informatif
Description
Le feedback doit :
Être rapide
Porter sur le processus, pas seulement le résultat
Permettre une correction immédiate
Rôle cognitif
Signal d’erreur indispensable à l’apprentissage
Ajustement des prédictions internes du cerveau
Conséquence pédagogique
Pas de feedback → pas de calibration → illusion de compétence

Pilier 4 — Répétition consciente et ajustée
Description
La répétition n’est jamais mécanique :
Chaque itération est légèrement ajustée
L’apprenant reste mentalement engagé
Rôle cognitif
Renforce les circuits pertinents
Élimine progressivement les stratégies inefficaces
Conséquence pédagogique
Répéter sans réfléchir ≠ pratiquer
-->

---

# Pourquoi les musiciens progressent mieux

- Répétition quotidienne
- Feedback immédiat
- Tolérance à l’erreur

> message à caractère intéressé : apprenez un instrument et rejoignez l'Union Musicale de Fontainebleau

<!-- speaker notes
Les musiciens ont intégré naturellement :

- la pratique quotidienne,  
- l’écoute immédiate de l’erreur (feedback),  
- et la tolérance à l’imperfection.

Leur cerveau s’adapte de manière visible. Des IRM ont montré des zones plus développées chez les musiciens experts (zones motrices, auditives…).

C’est un modèle de progression par **exigence douce**.

TRANSITION : Et dans le domaine pédagogique, il existe une approche qui respecte ces principes : TBR.
-->

---

# Training From The Back of the Room

## Apprentissage compatible cerveau - 4C

* Connexion
* Concept
* Pratique concrète
* Conclusion

<!-- speaker notes
**Sharon Bowman** a formulé cette méthode dans les années 2000. Elle repose sur les 4C :

1. **Connexion** : créer un lien avec le savoir antérieur.
2. **Concept** : introduire du contenu, en petites doses.
3. **Concret** : faire pratiquer immédiatement.
4. **Conclusion** : ancrer par reformulation et projection.

C’est un format anti-conférence passive, basé sur la **mobilisation cognitive immédiate**.

TRANSITION : L’IA pourrait être utilisée… pour favoriser ce type d’apprentissage. Ou l’inverse.
-->

---

# Alors… l’IA dans tout cela ?

## **Menace** ou **opportunité** ?

* Les deux
* L’IA amplifie votre posture, rien d'autre

<!-- speaker notes
Les deux.

On peut faire lever les gens pour voter

L’IA amplifie votre posture.
Rien d’autre.

L’IA est neutre dans son essence. Ce qu’elle amplifie, c’est **vous**.

Si vous cherchez à vous améliorer, elle sera un formidable outil.  
Si vous cherchez à vous simplifier, elle vous y aidera aussi.

Donc **la clé, c’est la posture**.

TRANSITION : Et ça veut dire que ce qu’on attend de vous demain… va changer.
-->

---

# Encore une bonne nouvelle

## Le niveau d’exigence va monter

* La vitesse seule ne suffit plus
* La valeur sera dans **?**

<!-- speaker notes
Ce qu’on attendra de vous dans quelques années, ce ne sera pas de produire vite.  
Ce sera de **comprendre**, **expliquer**, **relier** et **décider**.

La vitesse sera prise en charge par les IA.

Mais la **synthèse**, le **jugement**, la **créativité raisonnée**… ça restera votre valeur humaine.

TRANSITION : Encore faut-il ne pas tomber dans les pièges de la performance mal mesurée.
-->

---

# Un piège classique

## Les mauvaises métriques

> On obtient ce que l'on mesure

* Effet cobra
* Lignes de code
* Vitesse
* Volume

<!-- speaker notes
Un exemple célèbre : l’**effet cobra**. On récompensait les chasseurs de cobras à Delhi. Résultat : les habitants ont commencé à en élever chez eux pour toucher la prime.

L’intention était bonne, mais la **métrique mal pensée** a provoqué l’effet inverse.

En entreprise, c’est pareil : mesurer les mauvais indicateurs (ex : nombre de tickets fermés, volume de code produit…) peut conduire à dégrader la qualité.

Donc même avec l’IA, **le sens doit guider les mesures**.

TRANSITION : Et surtout, ne sacrifions pas l’essentiel.
-->

---

## Ne sacrifiez pas

* L’apprentissage
* L’esprit critique
* La joie de comprendre
* ...

<!-- speaker notes
L’IA peut vous aider à aller plus vite.
Mais ne sacrifiez pas ce qui vous construit profondément :
- votre capacité à apprendre,
- votre esprit critique,
- et surtout, votre plaisir à comprendre.

TRANSITION : Une dernière question, pour soi.
-->

---

# La question clé

## Quand j’utilise l’IA est-ce que
## **je gagne du temps** ou est-ce que **je progresse** ?

<!-- speaker notes
Posez-vous cette question à chaque fois que vous utilisez l’IA.  
Gagner du temps, c’est utile.
Mais progresser, c’est vital.

Et les deux ne vont pas toujours ensemble.

TRANSITION : Dernière mise au point.
-->

---
<!-- _class: concept -->
# Correction finale

## Augmenté vs amélioré était **un faux débat**

<!-- speaker notes
Ce n’était pas une opposition réelle.

Ce que nous avons opposé, c’était deux **postures**.

L’IA n’est ni bonne ni mauvaise.
Elle est **amplificatrice** de votre intention.

TRANSITION : D’où une responsabilité forte.
-->

---
<!-- _class: concept -->
# Liberté et responsabilité

## L’IA est puissante mais 
## **penser et décider reste votre rôle**

> A grands pouvoirs, grandes responsabilités

<!-- speaker notes
L’IA vous donne un pouvoir. Mais comme pour tout pouvoir, cela vient avec une responsabilité.

Vous êtes responsables de ce que vous validez.
De ce que vous signez.
De ce que vous pensez.

Et cette liberté, il faut la protéger activement.

TRANSITION : Merci !
-->

---

<!-- _class: lead -->
<!-- _paginate: skip -->

# Merci pour votre attention

## À votre disposition pour vos questions !

<!-- speaker notes
C’est le moment des questions.

Je préfère un vrai échange, une interrogation sincère, qu’un long monologue de conclusion.

Merci à tous et toutes pour votre écoute.
-->

---

Cette présentation est disponible ici :
[https://github.com/pypamart/conf-iep-fontainebleau-2026](https://github.com/pypamart/conf-iep-fontainebleau-2026)