# LIVRABLE 1 : Identification des Surfaces Fonctionnelles

## 1.1 Analyse du mecanisme

Le chapeau a pour fonction de :
- Maintenir le joint a levres en position
- Assurer l'etancheite dynamique (entre l'arbre tournant et le chapeau via le joint)
- Assurer l'etancheite statique (entre le chapeau et le carter)
- Etre fixe sur le carter par vissage

---

## 1.2 Surfaces fonctionnelles identifiees

| Ref | Surface | Fonction technique | Exigence geometrique | Rugosite Ra |
|-----|---------|-------------------|---------------------|-------------|
| **S1** | Alesage de logement du joint | Centrage et maintien radial du joint a levres | Cylindricite, Tolerance H8 | **Ra <= 3.2 um** |
| **S2** | Epaulement arriere (fond logement joint) | Appui axial du joint, positionnement | Planeite, Perpendicularite/S1 | **Ra <= 3.2 um** |
| **S3** | Face de contact avec le carter | Etancheite statique (avec joint torique ou pate) | Planeite | **Ra <= 0.8 um** |
| **S4** | Face d'appui sur le carter | Mise en position axiale du chapeau | Planeite, Parallelisme/S3 | **Ra <= 3.2 um** |
| **S5** | Trous de fixation (passage vis) | Assemblage demontable sur le carter | Position, Diametre | **Ra <= 6.3 um** |
| **S6** | Surfaces externes | Esthetique, protection corrosion | - | **Ra <= 12.5 um** |

---

## 1.3 Justifications (basees sur les annexes SKF)

### S1 - Alesage logement joint

- D'apres l'annexe "Joint a levres a contact radial" : pour une armature apparente (metal), **Ra <= 3.2 um** et **Rz <= 10 um**
- Tolerance sur le diametre : **H8** (ex: 40H8 pour un joint de diametre exterieur 40mm)
- Defaut de coaxialite maxi : 0.15 mm pour un arbre de 40mm

### S2 - Epaulement arriere

- Assure le positionnement axial du joint
- D'apres l'annexe SKF : "Axial faces of all grooves" **Ra <= 3.2 um**

### S3 - Face contact carter (etancheite statique)

- D'apres l'annexe "Rugosite etancheite" : les surfaces d'etancheite statique sous pression necessitent **Ra <= 0.8 um**
- Cette surface recoit soit un joint torique, soit de la pate d'etancheite

### S4 - Face d'appui

- Surface de reference pour le positionnement axial
- Necessite une bonne planeite pour garantir le serrage uniforme des vis

### S5 - Trous de fixation

- Fonction de passage de vis, pas d'exigence d'etancheite
- Rugosite standard de percage suffisante : **Ra <= 6.3 um**

---

## 1.4 Schema recapitulatif

```
                    S4 (Face appui)
                    |
    ________________|________________
   |                                 |
   |    S5 (Trous)      S5 (Trous)   |
   |        O               O       |
   |                                 |
   |     _______________________     |
   |    |                       |    |
   |    |   S1 (Alesage joint)  |    | S6 (Externe)
   |    |                       |    |
   |    |_______________________|    |
   |            S2 (Epaulement)      |
   |_________________________________|
                    |
                    S3 (Contact carter)
```

---

**Document realise dans le cadre du TD Design for Manufacturing - ESILV**
