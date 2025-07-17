Cet exposé a été réalisé par KOMARA LONCENY et CISSE M'BEMBA.

# Projet-sur-MATPLOTLIB
--------------------------------------------------------------------------------------------------------------
# Qu’est-ce que MATPLOTLIB ?
--------------------------------------------------------------------------------------------------------------
✅ bibliothèque de visualisation de données en Python.

✅ Utilité : tracer des graphiques statiques, interactifs ou animés.

✅ Module principal : pyplot, souvent importé sous le nom plt.

--------------------------------------------------------------------------------------------------------------
# Pourquoi utiliser MATPLOTLIB?
✅ 1. Visualiser facilement les données

      * Transforme les tableaux de chiffres en graphiques visuels faciles à comprendre.
      * Permet de repérer rapidement des tendances, des anomalies, ou des comparaisons.
✅ 2. Large choix de graphiques Matplotlib permet de tracer :

      * Courbes (plot)
      * Barres (bar)
      * Histogrammes (hist)
      * Camemberts (pie)
      * Nuages de points (scatter)
      * Courbes avec tendance (regplot via Seaborn)
✅ 3. Contrôle total sur le rendu

      * Tu peux personnaliser les couleurs, titres, tailles, styles, etc.
      * Tu peux ajouter des annotations, des grilles, des légendes, etc.
✅ 4. Intégration avec d'autres outils

     Compatible avec :
      * Pandas (pour analyser les données)
      * NumPy (pour manipuler des tableaux)
      * Seaborn (pour des graphiques plus stylés basés sur Matplotlib)
      * Jupyter Notebook (pour visualiser directement dans le cahier)
✅ 5. Gratuit et open-source

      * Tu peux l'utiliser sans licence, pour tous tes projets (perso, scolaire, pro).
--------------------------------------------------------------------------------------------------------------
# Cas d'utilisation

Pour commencer à utiliser Matplotlib dans un script Python, il faut importer la bibliothèque. Voici la syntaxe standard utilisée :
 
         import matplotlib.pyplot as plt
         
# # MODULE : MATPLOTLIB
--------------------------------------------------------------------------------------------------------------
# 1. Tracer une courbe simple (Graphique linéaire)
x = [1, 2, 3, 4, 5]

y = [2, 3, 5, 7, 11]

plt.plot(x, y, marker='o')

plt.title('Courbe simple')

plt.xlabel('x')

plt.ylabel('y')

plt.grid(True)

plt.show()

--------------------------------------------------------------------------------------------------------------
# 2. Histogramme

data = [1, 2, 2, 3, 3, 3, 4, 4, 4, 4, 5, 5]

plt.hist(data, bins=5, color='skyblue', edgecolor='black')

plt.title('Histogramme')

plt.xlabel('Valeurs')

plt.ylabel('Fréquence')

plt.show()

--------------------------------------------------------------------------------------------------------------
# 3. Graphique en barres

categories = ['A', 'B', 'C', 'D']

values = [10, 15, 7, 12]

plt.bar(categories, values, color='orange')

plt.title('Graphique en barres')

plt.xlabel('Catégories')

plt.ylabel('Valeurs')

plt.show()

--------------------------------------------------------------------------------------------------------------
# 4. Nuage de points (Scatter plot)

x = [1, 2, 3, 4, 5]

y = [5, 7, 4, 6, 9]

plt.scatter(x, y, color='red')

plt.title('Nuage de points')

plt.xlabel('x')

plt.ylabel('y')

plt.show()

--------------------------------------------------------------------------------------------------------------
# 5. Graphique en secteurs (camembert)

labels = ['Python', 'Java', 'C++', 'C#']

sizes = [40, 25, 20, 15]

plt.pie(sizes, labels=labels, autopct='%1.1f%%', startangle=140)

plt.title('Répartition des langages')

plt.axis('equal')  # Pour un cercle parfait

plt.show()

--------------------------------------------------------------------------------------------------------------
# 6. Droite de tendance avec une régression linéaire simple

import numpy as np

x = np.array([1, 2, 3, 4, 5])

y = np.array([2, 4, 5, 4, 5])

--------------------------------------------------------------------------------------------------------------
# Calcul des coefficients a et b pour y = ax + b

a, b = np.polyfit(x, y, 1)

plt.scatter(x, y, color='blue')

plt.plot(x, a*x + b, color='green', label=f'Tendance : y = {a:.2f}x + {b:.2f}')

plt.title('Droite de tendance')

plt.xlabel('x')

plt.ylabel('y')

plt.legend()

plt.grid(True)

plt.show()

--------------------------------------------------------------------------------------------------------------
Voir Image:
<img width="1550" height="1166" alt="image" src="https://github.com/user-attachments/assets/7ba52fb1-ea0e-45a3-89fb-daf60c240ddb" />
--------------------------------------------------------------------------------------------------------------
# Conclusion

Matplotlib s’impose comme une bibliothèque incontournable pour la visualisation de données en Python. Elle offre une grande flexibilité pour représenter graphiquement les relations statistiques et temporelles à travers divers types de graphiques tels que les histogrammes, les courbes linéaires, les barres, les nuages de points, ou encore les diagrammes en secteurs. Grâce à ses nombreuses fonctionnalités, elle permet non seulement d’explorer visuellement les données, mais aussi de communiquer efficacement les résultats d’analyse. Dans le cadre de cette étude, Matplotlib a permis de mettre en évidence les tendances et corrélations clés du marché automobile, facilitant ainsi la compréhension des facteurs influençant le prix des véhicules. Son intégration avec des bibliothèques comme Seaborn renforce encore sa puissance visuelle en rendant les graphiques plus esthétiques et informatifs.

--------------------------------------------------------------------------------------------------------------
# Remerciement:
Je tiens à vous exprimer ma profonde gratitude pour votre enseignement et votre accompagnement tout au long du cours de Data Mining. Grâce à votre pédagogie, votre disponibilité et votre passion pour la matière, j’ai pu mieux comprendre des concepts parfois complexes et enrichir considérablement mes compétences.
Merci pour le partage de vos connaissances, vos conseils précieux et pour l'attention que vous avez portée à nos projets. Votre implication a véritablement contribué à mon apprentissage et à ma motivation.
Avec tout mon respect et mes remerciements sincères.
