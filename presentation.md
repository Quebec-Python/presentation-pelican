# QuébecPython: première édition

## Présentation de Pelican

* http://docs.getpelican.com/

---

# Qui suis-je ?

* Je pars en voyage et j'apporte: Un des recueils de poésie de Gaston Miron
* Chanson que j'écouterai éternellement: *Aruarian Dance* de Nujabes
* Mon nom d'usager dans BZFlag: muymuy
* bernardchhun.com

---

# Pelican...c'est quoi ?

---

# C'est tout ?

---

# Comment ça fonctionne ?

<img style="width:100%" src="comment.png" />

---

# Pourquoi l'utiliser ?

* Nous sommes maître du *contenu* et du *contenant*
* Contenu en *Markdown*
* Hébergement sans soucis
    * Pas de base de données
    * Performant

---

# Performant ?

    !bash
    $ ab -n 500 -c 10 http://bernardchhun.com/
    # Requests per second:    70.30 [#/sec] (mean)
    # Time per request:       142.239 [ms]

    $ ab -n 500 -c 10 http://www.gc.ca/accueil.html
    # Requests per second:    26.75 [#/sec] (mean)
    # Time per request:       373.778 [ms]

* *-n* = nombre de requête
* *-c* = concurrence

---

# Pourquoi l'utiliser ?

* Bref, de la simplicité dans un monde complexe

---

# Ok, vendu.

---

# On commence par où ?

## Installation de la librairie

    !bash
    $ cd /votre/repertoire/favori
    $ virtualenv venv # optionnel
    $ source venv/bin/activate # optionnel
    $ pip install pelican

---

# Créer la structure de votre site

    !bash
    $ pelican-quickstart

---

# Créer un article

    !bash
    $ cd content
    $ touch un-article-magique.md
    $ vim un-article-magique.md

---

# Consulter votre site

    !bash
    $ make devserver

## Ouvrez ensuite votre navigateur à l'adresse http://localhost:8000

---

# Publier votre site via SSH

    !bash
    $ make ssh_upload

---

# Le thème de base est drabe.

## Créons-en un:

    !bash
    $ mkdir theme-qc-py

---

# Modifier la configuration

    !python
    #!/usr/bin/env python
    # -*- coding: utf-8 -*- #
    from __future__ import unicode_literals

    AUTHOR = u'Bernard Chhun'
    TAGLINE = u"Développeur web généraliste"
    AUTHOR_BIO = u"Père de famille, musicien, poête en devenir"
    SITENAME = u'Divagation et vagabondage'
    SITEURL = 'http://localhost:8000'
    # DÉBUT ICI !
    THEME = "./theme-qc-py"
    # FIN ICI !
    TIMEZONE = 'America/Montreal'

---

# Alternatives à Pelican

## http://modernstatic.com/

---

# Questions ?

---

# Merci !
