
---

## ✅ Qu’est-ce que l’analyse AS-IS ?

L’analyse **AS-IS** décrit l’**état actuel** du **Système d’Information (SI)** de l’entreprise — comment ça fonctionne aujourd’hui.

Elle inclut :

* **Les logiciels et outils existants** utilisés par l’entreprise
* **Les fonctions métiers** supportées par chaque outil (vente, finance, transport, etc.)
* **Comment ces systèmes communiquent (ou pas)**
* Les **limitations** ou **points de douleur** connus

Le but est de **comprendre la situation de départ** avant de recommander des changements.

---

### 🏢 Entreprise : LogiMed (Logistique & Transport International)

![image](bla2.png)

Ils utilisent actuellement :

1. **ERP** → Gestion financière
2. **WMS (Warehouse Management System)** → Gestion d’entrepôt
3. **TMS (Transport Management System)** → Expéditions et transport
4. **Logiciel sur mesure** → Suivi de la relation client

Mais ces outils sont :

* **Peu ou pas intégrés**
* Probablement des **manipulations manuelles** pour transférer les données entre systèmes
* Chaque système peut contenir des **données redondantes ou incohérentes**

---

## 🧩 Blocs fonctionnels AS-IS

| Domaine métier   | Outil existant      | Rôle/Fonction                     |
| ---------------- | ------------------- | --------------------------------- |
| Finance          | ERP                 | Comptabilité, facturation, budget |
| Entrepôt         | WMS                 | Stocks, stockage, inventaire      |
| Transport        | TMS                 | Itinéraires, suivi des livraisons |
| Ventes & Clients | Logiciel sur mesure | Commandes clients, communication  |
| RH (supposé)     | ERP ou manuel       | Paie, contrats                    |
| Direction        | Excel/email/manual  | Reporting, pilotage stratégique   |

---

## 🗺️ Cartographie fonctionnelle AS-IS (carte conceptuelle)

Une carte visuelle simplifiée pourrait ressembler à :

```
+-------------+       +------------+       +-------------+  
|   ERP       | <---> |  Finance   | <---> | Direction   |  
+-------------+       +------------+       +-------------+  

+-------------+       +-------------+  
|   WMS       | <---> | Entrepôt    |  
+-------------+       +-------------+  

+-------------+       +-------------+  
|   TMS       | <---> | Transport   |  
+-------------+       +-------------+  

+------------------+  +------------------+  
| Logiciel sur mesure|->| Relation Clients |  
+------------------+  +------------------+  

Tous les systèmes sont majoritairement isolés ; l’intégration est minimale ou manuelle.  
```

---
