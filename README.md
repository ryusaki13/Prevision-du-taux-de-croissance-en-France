# Analyse de l’impact de la croissance démographique sur la croissance économique en France  

> 🏫 Projet académique – Étude économique appliquée à la data science  

Ce projet explore la relation entre la **croissance démographique** et la **croissance économique** en France, à partir de données couvrant la période **1960 – 2023**.  
Il s’inscrit dans le cadre d’une **étude académique** combinant analyse économique et modélisation statistique.  

---

## Objectifs  
- Étudier les relations entre indicateurs **démographiques** et **macroéconomiques**.  
- Identifier les facteurs explicatifs du **PIB par habitant**.  
- Évaluer la pertinence de modèles statistiques (régression linéaire et séries temporelles).  

---

## Méthodologie et résultats  

### 1. **Analyse exploratoire des données (EDA)**  
**Variables étudiées** : PIB/habitant, croissance démographique, inflation, fiscalité, importations/exportations, mortalité infantile, IDE, solde migratoire, taux d’emploi, taux d’épargne, IDH, FBCF, natalité, mortalité, cycles économiques et politiques.  

**Points saillants** :  
- Le **PIB/habitant** croît globalement mais subit des chocs (crises économiques).  
- L’**inflation** est instable entre 1970 et 1985, puis se stabilise.  
- La **croissance démographique** est en déclin structurel.  
- Le **solde migratoire** chute dans les années 1980–90, puis repart à la hausse après 2000.  
- Le **taux d’emploi** atteint 69% sous la présidence Macron, un record historique.  
- Le **taux d’épargne** augmente en période de crise.  

---

### 2. **Régression linéaire**  
Modèle appliqué au **PIB par habitant**.  

**Résultats** :  
- +1% de croissance démographique → **–3,08 unités** de PIB/habitant.  
- La **FBCF** stimule positivement le PIB.  
- Le **taux d’emploi** influe négativement (emplois peu productifs).  
- La **fiscalité** pèse négativement et significativement sur le PIB.  

⚠️ **Limite** : modèle peu robuste, difficulté à intégrer les chocs économiques.  

---

### 3. **Modélisation en séries temporelles (SARIMAX)**  
Modèle choisi : **SARIMAX(1,0,3)** avec variables exogènes (**FBCF** et **taux d’épargne**).  

**Résultats** :  
- La **FBCF** et l’**épargne** influencent positivement le PIB/habitant.  
- Le PIB dépend fortement de sa propre valeur passée (**Ar.L1**).  
- La **croissance démographique** n’apparaît pas comme un déterminant significatif.  

⚠️ **Limite** : risque d’**overfitting** (modèle trop ajusté aux données d’entraînement).  

---

## Sources de données  
- **INSEE** – Données macroéconomiques françaises  
- **Banque mondiale** – Indicateurs du développement  
- **OCDE** – Statistiques économiques et sociales  
- **PNUD** – Indice de Développement Humain (IDH)  
- **Eurostat** – Indicateurs européens  

---

## Conclusion  
Cette étude montre que, dans le cas français, **la croissance démographique n’est pas un moteur direct de la croissance économique**.  
D’autres facteurs structurels tels que la **FBCF, le taux d’épargne et la fiscalité** jouent un rôle plus déterminant.  

---
