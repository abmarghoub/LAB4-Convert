# LAB 4 – Convertisseur Température & Distance (Fragments + Onglets)



---

## Réalisé par

**Abla MARGHOUB**

## Encadré par

**Pr. Mohamed LACHGAR**

## Module

**Techniques de Programmation Avancée**

## Établissement

**École Normale Supérieure - Université Cadi Ayyad**

---

## 1. Objectif du TP
L'objectif de ce TP est de réaliser une application Android composée de deux onglets :  

- **Température** : conversion °C ↔ °F  
- **Distance** : conversion Km ↔ Miles  

Fonctionnalités supplémentaires :  
- Afficher un menu “Quitter”  
- Intercepter la touche Retour pour demander confirmation avant de fermer l’application
---

## 2. Description des interfaces et classes

| Nom | Type | Rôle / Description |
|-----|------|------------------|
| `MainActivity` | Activity | Activité principale qui contient le `TabLayout` et le `ViewPager2`. Gère la confirmation de sortie. |
| `ViewPagerAdapter` | Adapter | Fournit les fragments correspondant aux onglets (`TempFragment` et `DistanceFragment`). |
| `TempFragment` | Fragment | Permet la conversion de température °C ↔ °F. Contient RadioButtons, EditText, Button et TextView pour afficher le résultat. |
| `DistanceFragment` | Fragment | Permet la conversion de distance Km ↔ Miles. Contient RadioButtons, EditText, Button et TextView pour afficher le résultat. |
| `activity_main.xml` | Layout | Layout principal contenant `TabLayout` et `ViewPager2`. |
| `fragment_temp.xml` | Layout | Layout du fragment Température avec saisie et résultat. |
| `fragment_distance.xml` | Layout | Layout du fragment Distance avec saisie et résultat. |

---

## 3. Fonctionnement global
1. L’application affiche deux onglets : Température et Distance.
2. Chaque onglet affiche un fragment indépendant avec sa zone de saisie et bouton de conversion. 
<img width="407" height="847" alt="image" src="https://github.com/user-attachments/assets/0be2b125-a1c2-4e1e-98cd-b35820be960e" />

3. L’utilisateur saisit une valeur, choisit le sens de conversion et clique sur "Calculer".
4. Le résultat s’affiche avec 2 décimales.  
<img width="500" height="875" alt="image" src="https://github.com/user-attachments/assets/199387c1-0c66-4d87-8185-d7ec97fa6559" />

5. Appuyer sur la touche **Retour** affiche une boîte de dialogue demandant confirmation avant de quitter.  

  <img width="405" height="743" alt="image" src="https://github.com/user-attachments/assets/f8f556d0-9b96-4657-8ab1-8288b304719c" />

---

## 4. Architecture technique

### 4.1 Stack technologique

| Technologie / Librairie | Version | Utilisation |
|-------------------------|---------|------------|
| Java | 1.8+ | Langage principal de développement |
| Android Studio | 2023+ | IDE |
| Android SDK | API 24+ | SDK minimum supporté |
| Material Components | 1.12.0 | Composants modernes (TabLayout, AlertDialog, etc.) |
| ViewPager2 | 1.0.0 | Gestion du défilement horizontal des fragments |
| AndroidX | 1.8+ | Support des fragments et compatibilité |

### 4.2 Structure du projet

<img width="492" height="635" alt="image" src="https://github.com/user-attachments/assets/f9894f66-32b1-4fe3-8a90-b820dde67ff7" />

---

## 5. Démonstration 

https://github.com/user-attachments/assets/852d3904-3a3c-462e-97ea-3ba05acc2024

---







