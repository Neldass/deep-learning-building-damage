# 🧠 Deep Learning – Building Damage Detection

Ce projet vise à automatiser la détection de bâtiments endommagés après une catastrophe naturelle, via des modèles de deep learning appliqués à des images satellites post-ouragan (*Harvey 2017*). Il s’appuie notamment sur la reproduction de l’étude de **[Cao and Choe, 2020]**.

---

## 📂 Contenu du dépôt

- 📁 `notebooks/` : implémentations en PyTorch
  - VGG-16 reproduit selon l’étude de Cao & Choe
  - Étude comparative des approches de transfert learning : Type A vs Type B
- 📁 `Rapport/` : le rapport complet du projet
  - 📄 [Projet Deep Learning_NKODIA Teddy.pdf](./Rapport/Projet%20Deep%20Learning_NKODIA%20Teddy.pdf)

---

## 📊 Résultats Clés

| Modèle         | Type       | Accuracy | AUC     | F1-score |
|----------------|------------|----------|---------|----------|
| VGG-16         | Fine-tuning| 94.55 %  | 0.989   | 0.9435   |
| DenseNet121    | Type B     | ~        | 0.9985  | 0.9844   |
| ResNet18       | Type A     | ~        | 0.9654  | 0.9040   |

> ⚠️ Les entraînements ont été limités à 10 époques pour des raisons de ressources.

---

## ⚙️ Environnement

torch
torchvision
scikit-learn
matplotlib
pandas
