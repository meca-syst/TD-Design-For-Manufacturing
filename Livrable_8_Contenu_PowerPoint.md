# LIVRABLE 8 : Contenu Presentation PowerPoint (5-10 min)

---

## SLIDE 1 - Page de titre

```
+--------------------------------------------------+
|                                                  |
|       TD : DESIGN FOR MANUFACTURING              |
|                                                  |
|   Conception d'un chapeau de maintien            |
|   de joint a levres                              |
|                                                  |
|   Famille de procedes : FONDERIE                 |
|                                                  |
|   Equipe : [Noms des membres]                    |
|                                                  |
|   ESILV - [Date]                                 |
|                                                  |
+--------------------------------------------------+
```

---

## SLIDE 2 - Contexte et objectifs

### Le mecanisme

- Chapeau de maintien d'un joint a levres
- Fonction : etancheite dynamique (arbre tournant) et statique (carter)

### Objectifs du TD

- Concevoir la piece en fonction du procede
- Proposer une gamme de fabrication
- Evaluer les couts

**[Inserer image : Vue 3D du mecanisme fourni dans le sujet]**

---

## SLIDE 3 - Surfaces fonctionnelles

### 6 surfaces identifiees :

| Surface | Fonction | Ra requis |
|---------|----------|-----------|
| S1 | Alesage logement joint | <= 3.2 um |
| S2 | Epaulement appui joint | <= 3.2 um |
| S3 | Contact carter (etancheite statique) | <= 0.8 um |
| S4 | Face d'appui sur carter | <= 3.2 um |
| S5 | Trous de fixation | <= 6.3 um |
| S6 | Surfaces externes | <= 12.5 um |

**[Inserer image : Dessin annote avec les surfaces reperees S1-S6]**

---

## SLIDE 4 - Choix du procede

### Procede retenu : Coulee en coquille par gravite (Gravity Die Casting)

| Critere | Fonderie | Forgeage | Emboutissage | Additif |
|---------|----------|----------|--------------|---------|
| Forme 3D creuse | OUI | NON | LIMITE | OUI |
| Cout (1000 pcs) | 23-51 EUR | 27-50 EUR | 18-38 EUR | 103-3790 EUR |
| Ra brut | 3.4-6.3 um | 3.2-12.5 um | 0.8-3.2 um | Variable |

### Justification :

- Geometrie adaptee (piece creuse avec alesage)
- Cout optimal en moyenne serie
- Compatible aluminium

---

## SLIDE 5 - Conception du chapeau

### Regles de conception fonderie :

| Parametre | Valeur |
|-----------|--------|
| Depouilles | 5 degres |
| Epaisseur uniforme | 8-10 mm |
| Rayons de raccordement | R >= 3 mm |
| Surepaisseurs usinage | 1.5 mm |

**[Inserer image : Dessin du brut de fonderie vs piece finie]**

---

## SLIDE 6 - Gamme de fabrication

```
FONDERIE (Phase 10)
       |
       v
PARACHEVEMENT (Phase 20)
       |
       v
TOURNAGE (Phase 40) --> S1, S2, S4
       |
       v
FRAISAGE (Phase 50) --> S3
       |
       v
PERCAGE (Phase 60) --> S5
       |
       v
RECTIFICATION (Phase 70) --> S3 (optionnel)
       |
       v
CONTROLE (Phase 90)
```

---

## SLIDE 7 - Procedes secondaires

| Surface | Ra requis | Ra brut | Procede | Justification |
|---------|-----------|---------|---------|---------------|
| S1 | 3.2 um | 3.4-6.3 um | Tournage finition | Logement joint |
| S2 | 3.2 um | 3.4-6.3 um | Tournage | Appui joint |
| S3 | 0.8 um | 3.4-6.3 um | Surfacage + Rectif. | Etancheite statique |
| S5 | 6.3 um | N/A | Percage | Trous non moulables |

**Source : Annexes SKF et Rugosite**

---

## SLIDE 8 - Materiau

### Alliage choisi : AS7G (AlSi7Mg / A356)

| Propriete | Valeur |
|-----------|--------|
| Densite | 2.68 g/cm3 |
| Rm | 250-290 MPa |
| Re | 180-220 MPa |
| Durete | 75-90 HB |

### Justification :

- Excellente coulabilite
- Bonne usinabilite
- Leger (3x moins que acier)
- Resistant a la corrosion
- Cout modere (7 EUR/kg)

---

## SLIDE 9 - Analyse economique

### Seuil de rentabilite : ~500 pieces

| Quantite | Cout/piece |
|----------|------------|
| 100 | 140 EUR |
| 500 | 45 EUR |
| 1 000 | **34-80 EUR** |
| 10 000 | **28-60 EUR** |

### Batch economique : 1 000 - 100 000 pieces

**[Inserer image : Courbe cout vs quantite de GRANTA EDUPACK]**

---

## SLIDE 10 - Conclusion

### Resume :

| Element | Choix |
|---------|-------|
| Procede | Fonderie coquille par gravite |
| Materiau | Aluminium AS7G |
| Quantite rentable | >= 500 pieces |
| Cout estime | 40-50 EUR/piece (1000-10000 pcs) |

### Avantages de la solution :

- Bon compromis cout/qualite
- Piece legere et resistante a la corrosion
- Usinage limite aux surfaces fonctionnelles

### Questions ?

---

## Notes pour l'oral

### Timing suggere :

| Slide | Duree | Contenu |
|-------|-------|---------|
| 1 | 30 sec | Presentation equipe |
| 2 | 1 min | Contexte |
| 3 | 1 min 30 | Surfaces fonctionnelles |
| 4 | 1 min 30 | Choix procede |
| 5 | 1 min | Conception |
| 6 | 1 min | Gamme |
| 7 | 1 min 30 | Procedes secondaires |
| 8 | 1 min | Materiau |
| 9 | 1 min | Economie |
| 10 | 1 min | Conclusion |
| **Total** | **~10 min** | |

### Points cles a souligner :

1. Coherence entre exigences fonctionnelles et choix du procede
2. Justification des operations d'usinage par les rugosites requises (annexes)
3. Compromis cout/qualite/quantite
4. Comparaison avec les autres familles de procedes

---

**Document realise dans le cadre du TD Design for Manufacturing - ESILV**
