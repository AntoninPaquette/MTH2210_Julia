# Génération d'un pdf

Le package [Weave](http://weavejl.mpastell.com/stable/) permet de générer un
rapport sous format pdf d'un script Julia.

Le fichier [gabarit_rapport.jl](../../src/gabarit_rapport.jl) est un gabarit de rapport.
Après avoir édité votre script, vous pouvez publiez votre script en format pdf
(avec pdflatex) avec la commande
```julia
weave("gabarit_rapport.jl", doctype = "md2pdf")
```
ou en format HTML avec la commande
```julia
weave("gabarit_rapport.jl", doctype = "md2html").
```
Il est important d'imprimer ensuite le fichier HTML en format pdf pour la remise
sur Moodle.

La ligne de code précédente ne doit pas se retrouver dans votre script. Vous
devez l'éxécuter dans la console de Julia en vous assurant d'être dans le
bon dossier.