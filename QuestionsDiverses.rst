Questions diverses
""""""""""""""""""

Les hotspots :
==============

- Hotspot dual band : On peut configurer deux fréquences différentes pour RX et TX, le hotspot passe pour relais
- Hotspot single band : Mode dmo. Utiliser une seule fréquence RX/TX sinon pas de cnx possible au master. Le master vérifie la config.

Il n'est pas necessaire d'avoir un ID à 6 chiffres pour utiliser un hotspot
Utiliser un SSID par hotspot permet de différencier les configurations dans selfcare.
Dès qu'on a un ssid, le hotspot arrive direct dans le selfcare.
Si des ssid ont été déclarés et ne sont pas utilisés, il sont nettoyés tous les 3 mois.

Pour que les SMS fonctionnent sur un hotspot/relais MMDVM, il est nécessaire de désactiver la confirmation des 
appels Data dans le codeplug de votre poste, ce réglage est dans les paramètres de chaque canal. 
(Chez Motorola, il s'agit de la fonction Data Call Confirmed).
Attention, dans ce cas de figure, il est nécessaire de désactiver l'option "Text Capture" dans votre Selfcare, ou vous 
recevrez sans cesse les messages en attente.


Conseils concernant les codeplugs
================================

Concernant la programmation d'un codeplug, j'ai vu passer quelques codeplugs avec de nombreux canaux pour le même relais,
ce qui complique inutilement le codeplug dès que vous avez quelques relais.
Inga YL3IM a très bien résumé la logique à suivre pour programmer votre codeplug.
Un canal, c'est :
    - Une fréquence (ou un couple pour un relais).
    - Un code couleur.
    - Un time slot.
    - Une rx list contenant les groupes à recevoir.
    - Un contact par défaut.

En suivant cette logique, vous aurez un codeplug plus leger. La rx group list va vous permettre de recevoir vos correspondants
quel que soit le TG sur lequel ils se trouvent tant que ce TG figure dans votre rx group list.
Si vous appuyez sur le bouton PTT immédiatement après avoir reçu un appel sur un TG qui n'est pas le TG par défaut configuré
sur votre canal, votre poste va se mettre automatiquement sur le TG qui a appelé et va y rester quelques secondes 
(délai configuré dans votre codeplug) vous permettant ainsi de faire le qso. Si vous désirez appeler sur un TG
que celui qui est défini par défaut, il suffit de le sélectionner dans vos contacts et de presser le bouton PTT.



