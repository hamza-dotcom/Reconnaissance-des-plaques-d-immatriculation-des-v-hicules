
## Exigences

Afin de pouvoir exécuter facilement le code, vous devez avoir installé le framework Keras avec le backend TensorFlow. Le framework Darknet est contenu dans le dossier "darknet" et doit être compilé avant d'exécuter les tests. Pour compiler Darknet, tapez simplement "make" dans le dossier "darknet" :

``shellscript
$ cd darknet && make
```

**La version actuelle a été testée sur une machine Ubuntu 16.04, avec Keras 2.2.4, TensorFlow 1.5.0, OpenCV 2.4.9, NumPy 1.14 et Python 2.7.**.

## Télécharger les modèles

Après avoir construit le framework Darknet, vous devez exécuter le script "get-networks.sh". Ceci téléchargera tous les modèles formés :

``shellscript
$ bash get-networks.sh
```

##Executer un test simple

Utilisez le script "run.sh" pour exécuter notre approche ALPR. Il requiert 3 arguments :
* __Répertoire d'entrée (-i):__ doit contenir au moins 1 image au format JPG ou PNG ;
* __Répertoire de sortie (-o):__ pendant le processus de reconnaissance, de nombreux fichiers temporaires seront générés dans ce répertoire et effacés à la fin. Les fichiers restants seront liés à l'image annotée automatiquement ;
* __Fichier CSV (-c):__ spécifier un fichier CSV de sortie.






Traduit avec www.DeepL.com/Translator (version gratuite)