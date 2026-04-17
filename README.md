# KanBan Project

## apercu visuel

### accueil

![Accueil](screenshots/home-page.png)

Page d entree avec acces rapide a la creation de projet et a la liste des projets.

### board kanban

![Board Kanban](screenshots/kanban-board.png)

Vue principale du board avec colonnes, deplacement des stories et actions rapides.

### board avec swimlanes

![Board avec swimlanes](screenshots/board-with-swimlanes.png)

Organisation visuelle par swimlanes pour separer les flux d un meme projet.

### creation de projet

![Creation projet](screenshots/create-project-form.png)

Formulaire de creation de projet avec validations de base.

### ajout de story

![Ajout de story](screenshots/add-story-modal.png)

Creation rapide d une story depuis le board.

### detail story et timer

![Detail story et timer](screenshots/story-detail-time-tracking.png)

Fiche story avec suivi du temps, timer start/stop et historique des worklogs.

### exemple de workflow

![Exemple workflow](screenshots/workflow-example.png)

Exemple de workflow avec colonnes et progression des stories.

## presentation du projet

Projet de gestion de taches en mode Kanban, developpe en Java avec Spring MVC.

Le projet permet de creer des projets, gerer des stories, organiser le travail par colonnes et swimlanes, et suivre le temps passe sur chaque story.

## ce que fait le projet

- creation, edition et suppression de projets
- creation automatique des colonnes de base: BACKLOG, IN PROGRESS, REVIEW, DONE, BLOCKED
- board Kanban avec deplacement des stories entre colonnes
- colonnes personnalisees avec capacite max (WIP limit)
- sous-colonnes Backlog/Done pour certaines colonnes
- gestion des swimlanes par projet
- gestion des stories: creation, edition, suppression, assignation
- timer et worklogs (demarrer, arreter, ajout manuel, historique)
- tests unitaires + tests d integration

## stack technique

- java 17
- maven (multi-modules)
- spring mvc 5
- thymeleaf
- bootstrap 5
- architecture en memoire (pas de base SQL)
- junit 5, mockito, selenium, webdrivermanager
- jacoco, spotbugs, pitest

## structure du projet

```text
gestiondetaches/
├── tarnished/
│   ├── project-model/      # entites metier
│   ├── project-repomem/    # repositories en memoire
│   └── project-app/        # controllers + vues web
├── screenshots/            # captures README
├── .gitignore
├── .gitlab-ci.yml
└── README.md
```

## installation et lancement

### prerequis

- java 17
- maven 3.9+

### build

Depuis le dossier `tarnished`:

```bash
mvn clean install
```

### lancer l application

Depuis `tarnished/project-app`:

```bash
mvn jetty:run
```

Puis ouvrir:

- http://localhost:8080/gl2526-tarnished

### tests

Depuis `tarnished`:

```bash
mvn test
```

Pour les tests d integration:

```bash
mvn verify
```

## resume pour portfolio

Description courte:

Application web Kanban en Java (Spring MVC) pour piloter des projets et stories, avec board drag and drop, swimlanes, et suivi du temps par story.

Stacks:

Java 17, Spring MVC, Thymeleaf, Bootstrap, Maven, JUnit, Mockito, Selenium.

Role du projet:

Projet de genie logiciel centre sur la modelisation metier, l architecture multi-modules et les tests (unitaires + integration).

### bloc pret a copier dans le portfolio

Description:

Application Kanban Java pour gerer projets et stories avec board interactif, swimlanes et suivi du temps.

Stacks:

Java 17, Spring MVC, Thymeleaf, Bootstrap, Maven, JUnit, Mockito, Selenium.

Role:

Conception et implementation d une application web de gestion de taches en architecture multi-modules, avec logique metier testee.

## github et collaboration

### start coding with codespaces

Le projet peut etre lance dans GitHub Codespaces. Une fois l environnement ouvert:

- verifier Java 17 et Maven
- executer `mvn clean install` dans `tarnished`
- executer `mvn jetty:run` dans `tarnished/project-app`

### add collaborators

Sur GitHub:

- ouvrir le repository
- aller dans Settings > Collaborators and teams
- ajouter les collaborateurs par username GitHub ou email

### quick setup

Repository cible:

- https://github.com/ZakBZD100/KanBan-Project.git

Creer un repo:

```bash
echo "# KanBan-Project" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/ZakBZD100/KanBan-Project.git
git push -u origin main
```

Push un projet existant:

```bash
git remote add origin https://github.com/ZakBZD100/KanBan-Project.git
git branch -M main
git push -u origin main
```

## collaborateurs

- Zakariae El Bouzidi
- Nabil Dahmani
- Hamza Fikri
- Moncef Hiam
- Louay BEN El Toufa

## licence

Ce projet est distribue sous licence MIT. Voir le fichier LICENSE.

Zakariae El Bouzidi 2026

