# Journal des versions

## v3.1 — juillet 2026
- Rémunération simplifiée : règle unique automatique — 1 €/boîte si l'objectif (ou le 1er palier défini) est atteint, sinon 0 ; primes de paliers cumulées ; barème produits (boîtes × montant) prioritaire quand les quantités sont renseignées.
- Répartition : arrondi automatique à l'euro inférieur, report calculé automatiquement avec indication du laboratoire où reste le solde, mémorisation du report et case « Utiliser le report » à la dispatch suivante, plan de versement conseillé affiché (virements regroupés par laboratoire).
- Période et progression calculées uniquement sur les challenges actifs (les instantanés d'une période précédente sont ignorés).
- Export PDF : capture consolidée (correctif du cadre décalé).

## v3.0 — juillet 2026
- Correction de l'impression navigateur (Chrome, Firefox, Brave…) : pages du rapport alignées et à taille réelle grâce à une mise en page d'impression dédiée (format A4 sans marges, centrage et zoom mobile neutralisés, sauts de page propres). L'impression de la Répartition garde ses marges de feuille.
- Révision du code : règles d'impression consolidées (doublons supprimés), styles inutilisés retirés.

## v2.9 — juillet 2026
- Répartition : versements en euros entiers (un seul virement rond par personne), champ « montant à déduire / report » et reliquat « à reporter », bouton « Copier le plan de versement ».
- Postes personnalisables : ajout, renommage et suppression de postes.
- Logos de laboratoires fournis (dossier `logos/`) et sélecteur « Logos fournis » sur chaque fiche.

## v2.8 — juillet 2026
- Icône d'écran d'accueil : le logo s'affiche désormais quand l'application est ajoutée à l'accueil d'un iPhone (apple-touch-icon) ou d'un Android (manifest).

## v2.7 — juillet 2026
- Correction de l'export PDF : contenu décalé vers la droite et tronqué, et pages blanches intercalées. La génération utilise désormais une mise en page de capture dédiée (alignement, marges et ombres neutralisés).

## v2.6 — juillet 2026
- Optimisations : collecte des données une seule fois par rendu, sauvegarde ignorée quand rien n'a changé (moins d'écritures disque), et la saisie dans la page Répartition ne re-génère plus l'aperçu du rapport ni la date de dernière saisie des challenges.

## v2.5 — juillet 2026
- Période globale du rapport : du début le plus ancien des challenges en cours à la date de fin la plus fréquente (ex. 3 fins au 31/08 et 1 au 30/09 → 31/08). Les challenges expirés sont ignorés.

## v2.4 — juillet 2026
- Affichage adapté au mobile : mise en page en colonne, aperçu du rapport mis à l'échelle de l'écran, tableau de répartition défilable, boutons et grilles réorganisés.
- Logo de l'application (SVG + PNG) et icône d'onglet (favicon).
- Fichier livré vierge : aucune donnée d'exemple pré-remplie au premier lancement.

## v2.3 — juin 2026
- Retrait des modèles de barèmes propres à un fournisseur : la rémunération « € par boîte » se paramètre librement (tranches, booster, minimum).
- Préparation à la publication : dépôt GitHub (README, licence MIT, journal des versions).

## v2.2 — juin 2026
- Répartition : ajout de laboratoires/challenges directement dans le dispatch (lignes libres).
- Pondération par les heures travaillées avec un référentiel temps plein paramétrable (ex. 10 h / 35 h).

## v2.1 — juin 2026
- Répartition : case « Participe » pour inclure ou exclure une personne de la distribution en cours sans la retirer de l'effectif ; ajout / retrait de personnes.

## v2.0 — juin 2026
- Nouvelle page « Répartition des gains » : sélection des challenges et de leurs montants, dispatch par personne (nom, prénom, email, poste), pondération par poste (onglet Paramètres), suivi total à verser / déjà versé / reste. Impression et export CSV dédiés.

## v1.9 — juin 2026
- Rémunération « par produit » : saisie des boîtes vendues par produit (× barème), additionnée et comptée une fois le challenge validé. À défaut de détail par produit : 1 €/boîte vendue.

## v1.8 — juin 2026
- Aide intégrée (bouton ⓘ) et journal des nouveautés.
- Optimisations internes (calculs mis en cache) et neutralisation de l'injection de formule à l'export CSV.

## v1.7
- Gains acquis vs gains estimés (projection de fin de période), récapitulatif global et estimation du déblocage du minimum.

## v1.6
- Moteur de rémunération « € par boîte » : tranches marginales, booster et minimum conditionnant le paiement.

## v1.5
- Paliers de challenge (stepper) et encart « Produits challengés » avec montants associés.

## v1.4
- Saisie mensuelle alignée sur le logiciel métier, projection au rythme mensuel, suivi des mises à jour hebdomadaires et écart depuis la dernière saisie.

## v1.3
- Refonte du PDF : identité officine, jauges de progression, page de couverture et podium.

## v1.2
- Logos locaux (importer / glisser-déposer / coller), bibliothèque réutilisable, SVG vectoriel + compression, jauge de stockage.

## v1.1
- Indicateur de rythme, mode comptoir (+1/+5), historique & tendance, nouvelle période, annulation de suppression, mode hors-ligne.

## v1.0
- Version initiale : suivi des challenges, indicateurs clés, tri, export JSON/CSV, génération PDF.
