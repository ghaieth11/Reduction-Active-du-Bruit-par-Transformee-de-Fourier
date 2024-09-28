# Réduction Active du Bruit en Utilisant la Transformée de Fourier

## Introduction

Ce projet vise à diminuer le bruit en milieu urbain en utilisant des techniques de traitement du signal basées sur la transformée de Fourier. L'objectif est de capturer un signal sonore primaire (bruit) et de générer un signal secondaire qui interfère destructivement avec le premier pour réduire le niveau de bruit.

Le processus repose sur l'idée de **Contrôle Actif du Bruit (ANC)**, où une onde sonore secondaire, déphasée par rapport à la première, est générée pour interférer destructivement avec l'onde initiale.

## Objectifs

- **Capture du bruit** : Utilisation de microphones pour enregistrer un signal sonore.
- **Analyse fréquentielle** : Application de la transformée de Fourier pour extraire les fréquences du bruit.
- **Génération du signal secondaire** : Création d'un signal en opposition de phase avec les mêmes fréquences.
- **Interférence destructrice** : Combinaison des deux signaux pour obtenir une réduction significative du bruit.

## Théorie

### Transformée de Fourier

La **transformée de Fourier** permet de transformer un signal temporel en un spectre fréquentiel. Ce processus décompose un signal complexe en une somme de sinusoïdes de différentes fréquences, amplitudes et phases.

L'équation de la transformée de Fourier est donnée par :
\[ F(f) = \int_{-\infty}^{\infty} f(t) e^{-2 \pi i f t} dt \]

L'inverse de la transformée de Fourier permet de reconstruire le signal temporel :
\[ f(t) = \int_{-\infty}^{\infty} F(f) e^{2 \pi i f t} df \]

### Contrôle Actif du Bruit

Le contrôle actif consiste à capter un bruit et à générer un signal inverse qui, lorsqu'il est superposé au bruit d'origine, interfère destructivement avec celui-ci. L'interférence destructive permet de réduire considérablement le niveau sonore perçu.

## Prérequis

- Python 3.x
- Bibliothèques : `numpy`, `scipy`, `matplotlib`, `sounddevice`

Installez les bibliothèques avec la commande suivante :

```bash
pip install numpy scipy matplotlib sounddevice
