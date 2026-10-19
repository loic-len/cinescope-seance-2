# CinéScope - TP : réparer la fenêtre modale

## Note de livrable

### Trois problèmes rencontrés

1. Bouton Réserver non focusable et sans nom accessible
2. Bouton de fermeture de la modal en <span onClick> ce qui est invisible au clavier et sans nom accessible, il n'est pas non plus possible de sortir de la modal en utilisant echap
3. Focus jamais déplacé, on pouvait accéder au contenu en arrière plan quand la modal était ouverte. Quand la model se ferme le focus sur la page n'est pas clair et fixe

### Impact utilisateur

1. Un utilisateur au clavier ne pouvait pas atteindre ni activer le bouton Réserver
2. Impossible de fermer au clavier via la croix, et le lecteur d'écran annonçait un élément sans nom
3. Un utilisateur clavier / lecteur d'écran pouvait tabuler « derrière » la modal et se perdre, après fermeture de la modal, le focus repartait en haut de page au lieu de revenir au film demandé ce qui pouvait egalement perdre l'utilisateur 

### Méthode de vérification pour chaque correction

- Clavier seul : Tab jusqu'au film « Après l'aube », Entrée pour ouvrir, Tab dans les
  commandes, Echap puis bouton × pour fermer, contrôle visuel du focus.
- Panneau Accessibilité : relevé du rôle dialog et du nom calculé
  du dialogue, et du bouton de fermeture.
- Test sur deux films successifs pour confirmer que le focus revient au bouton
  « Réserver » exact.

