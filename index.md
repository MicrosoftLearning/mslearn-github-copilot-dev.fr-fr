---
title: Instructions de l’exercice
permalink: index.html
layout: home
---

# Exercices GitHub Copilot

Les exercices de démarrage rapide suivants sont conçus pour vous offrir une expérience d’apprentissage pratique qui vous permettra d’explorer les fonctionnalités de GitHub Copilot. Chaque exercice comprend un ensemble de tâches que vous pouvez réaliser dans votre environnement de labo.

## Exercices de démarrage rapide
<hr>

{% assign labs = site.pages | where_exp:"page", "page.url contains '/Instructions/Labs'" %}

{% for activity in labs  %}

### [{{ activity.lab.title }}]({{ site.github.url }}{{ activity.url }})
{{ activity.lab.description }}
<hr>
{% endfor %}
