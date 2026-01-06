# LIVRABLE 4 : Justification des Procedes Secondaires/Tertiaires

## 4.1 Tableau de synthese

| Surface | Fonction | Ra requis | Ra brut fonderie | Procede secondaire | Justification |
|---------|----------|-----------|------------------|-------------------|---------------|
| **S1** | Logement joint | <= 3.2 um | 3.4-6.3 um | **Tournage finition** | Ra brut insuffisant |
| **S2** | Epaulement joint | <= 3.2 um | 3.4-6.3 um | **Tournage dressage** | Planeite et Ra |
| **S3** | Contact carter | <= 0.8 um | 3.4-6.3 um | **Surfacage + Rectif.** | Etancheite statique |
| **S4** | Face appui | <= 3.2 um | 3.4-6.3 um | **Tournage dressage** | Positionnement |
| **S5** | Trous fixation | <= 6.3 um | N/A | **Percage** | Non moulable |
| **S6** | Externes | <= 12.5 um | 3.4-6.3 um | **Aucun** | Ra suffisant |

---

## 4.2 Justifications detaillees

### S1 - Alesage logement joint (Tournage finition)

**Exigence :** Ra <= 3.2 um (source : Annexe SKF - armature apparente metal)

**Ra obtenu en fonderie :** 3.4 - 6.3 um --> **NON CONFORME**

**Procede choisi :** Tournage de finition (alesage)

**Justification :**
- Le tournage de finition permet d'obtenir Ra = 0.8 - 3.2 um
- Permet egalement de garantir la tolerance H8 sur le diametre
- La cylindricite obtenue (< 0.02 mm) garantit le centrage correct du joint
- Operation realisable en une seule prise sur tour CN

**Parametres de coupe suggeres :**
| Parametre | Valeur |
|-----------|--------|
| Vitesse de coupe | 200-300 m/min |
| Avance | 0.05 - 0.1 mm/tr |
| Profondeur de passe | 0.2 - 0.5 mm |

---

### S2 - Epaulement arriere (Tournage dressage)

**Exigence :** Ra <= 3.2 um (source : Annexe SKF - "Axial faces of all grooves")

**Ra obtenu en fonderie :** 3.4 - 6.3 um --> **LIMITE**

**Procede choisi :** Tournage dressage

**Justification :**
- L'epaulement assure le positionnement axial du joint
- Le tournage garantit la perpendicularite par rapport a l'alesage S1 (meme prise)
- Permet d'atteindre Ra = 1.6 - 3.2 um
- Indispensable pour eviter les fuites par defaut d'appui

---

### S3 - Face contact carter (Surfacage + Rectification)

**Exigence :** Ra <= 0.8 um (source : Annexe Rugosite - etancheite statique sous pression)

**Ra obtenu en fonderie :** 3.4 - 6.3 um --> **NON CONFORME**

**Procedes choisis :**

| Etape | Procede | Ra obtenu |
|-------|---------|-----------|
| 1 | Surfacage (fraisage) | 1.6 - 3.2 um |
| 2 | Rectification plane | 0.4 - 0.8 um |

**Justification :**
- Cette surface assure l'etancheite statique avec le carter
- Sans joint torique, la pate d'etancheite necessite Ra <= 0.8 um
- Le surfacage seul est insuffisant, la rectification est necessaire

**Alternative economique :**
Si un joint torique est utilise entre le chapeau et le carter, Ra <= 3.2 um suffit et la rectification peut etre supprimee.

---

### S4 - Face d'appui (Tournage dressage)

**Exigence :** Ra <= 3.2 um, planeite

**Ra obtenu en fonderie :** 3.4 - 6.3 um --> **LIMITE**

**Procede choisi :** Tournage dressage

**Justification :**
- Surface de reference pour la mise en position axiale
- Doit etre parallele a S3 pour garantir un serrage uniforme
- Tournage en meme prise que S1 et S2 pour garantir les tolerances geometriques

---

### S5 - Trous de fixation (Percage)

**Exigence :** Ra <= 6.3 um, position

**Ra obtenu en fonderie :** Non realisable (brut plein)

**Procede choisi :** Percage sur fraiseuse CN

**Justification :**
- Les trous ne sont pas realisables en fonderie (contre-depouilles)
- Le percage standard donne Ra = 3.2 - 6.3 um --> **CONFORME**
- La fraiseuse CN garantit la position precise des trous (repetition circulaire)
- Possibilite d'ajouter un lamage pour vis CHC

---

### S6 - Surfaces externes (Aucun usinage)

**Exigence :** Ra <= 12.5 um (esthetique)

**Ra obtenu en fonderie :** 3.4 - 6.3 um --> **CONFORME**

**Procede choisi :** Aucun (brut de fonderie)

**Justification :**
- Les surfaces externes n'ont pas de fonction d'etancheite ou de guidage
- La rugosite brute de fonderie est acceptable
- Grenaillage optionnel pour ameliorer l'aspect

---

## 4.3 Capabilites Ra par procede

| Procede | Ra atteignable (um) | Surfaces concernees |
|---------|---------------------|---------------------|
| Fonderie coquille (brut) | 3.4 - 6.3 | S6 |
| Tournage ebauche | 3.2 - 12.5 | - |
| Tournage finition | 0.8 - 3.2 | S1, S2, S4 |
| Fraisage/Surfacage | 1.6 - 6.3 | S3 (ebauche) |
| Percage | 3.2 - 6.3 | S5 |
| Rectification plane | 0.2 - 0.8 | S3 (finition) |

---

## 4.4 Sources utilisees

- Annexe "Joint a levres a contact radial" (SKF)
- Annexe "Rugosite etancheite"
- Fiches GRANTA EDUPACK

---

**Document realise dans le cadre du TD Design for Manufacturing - ESILV**
