# qTest
quizz_sur_l_informatique_quantique
Pour faire pivoter le qubit d’un angle de 120 degrés, nous devons utiliser la porte de rotation Z avec un angle de 240 degrés, car Z(θ) effectue une rotation de l’angle θ autour de l’axe Z.

Ainsi, le code qui doit remplacer « #Your code here » est :

qc.rz(240/180*pi, q[0])

Ici, nous utilisons la méthode rz() de l’objet QuantumCircuit pour appliquer une rotation autour de l’axe Z. L’angle de rotation est spécifié en radians, donc nous convertissons 120 degrés en radians en le multipliant par pi/180. Notez que nous divisons également par 180 pour simplifier la fraction.

Enfin, nous mesurons le qubit comme dans le code d’origine:

qc.measure(q,c)

Notez que la mesure ne modifie pas l’état quantique du qubit, elle ne fait que renvoyer une valeur classique correspondant à l’état quantique observé.
