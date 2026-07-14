# VHDL-Mini-Project
💡 Qu'est-ce que le VHDL ?
VHDL est l'acronyme de Very High Speed Integrated Circuit Hardware Description Language (langage de description de matériel). C'est un langage de programmation spécialisé qui permet de décrire le comportement et la structure d'un circuit électronique numérique, comme un processeur ou une puce FPGA . Contrairement aux langages de programmation classiques (comme C ou Python) qui décrivent une séquence d'instructions pour un processeur, le VHDL décrit un circuit physique constitué de portes logiques et de connexions .

⚙️ Pourquoi utiliser ModelSim ?
ModelSim est un logiciel de simulation. Le VHDL étant un langage de description, il ne peut pas être exécuté directement comme un programme classique. Il faut d'abord le "compiler" pour créer une base de données que le simulateur peut interpréter . ModelSim permet donc de :

Compiler votre code VHDL pour détecter les erreurs de syntaxe .

Simuler le comportement de votre circuit en lui envoyant des signaux d'entrée et en observant ses sorties sous forme de chronogrammes (waveforms) .

Déboguer votre conception en vérifiant son fonctionnement avant de la synthétiser sur un composant physique réel .

🚀 Comment utiliser VHDL avec ModelSim (Guide Pas à Pas)
Voici les étapes typiques pour mener à bien un projet VHDL avec ModelSim :

Créer un Projet : Lancez ModelSim, puis allez dans File > New > Project . Donnez un nom à votre projet et choisissez un répertoire de travail.

Ajouter vos Fichiers VHDL : Une fenêtre s'ouvre pour ajouter des fichiers. Vous pouvez y créer de nouveaux fichiers VHDL (Create New File) ou ajouter des fichiers existants (Add Existing File) . Vos fichiers de conception et votre "testbench" (un banc de test qui simule l'environnement de votre circuit) doivent porter l'extension .vhd ou .vhdl .

Compiler le Code : Avant de simuler, il faut compiler. Dans l'interface, sélectionnez Compile > Compile All . ModelSim compile tous les fichiers de votre projet .

Un ✔️ (coche verte) signifie que la compilation a réussi .

Une ❌ (croix rouge) indique une erreur ; vous pouvez cliquer dessus dans la fenêtre Transcript pour avoir plus de détails et corriger votre code .

Lancer la Simulation : Une fois la compilation réussie, allez dans Simulate > Start Simulation . Une fenêtre s'ouvre ; déroulez la bibliothèque work et sélectionnez l'entité à simuler, qui est généralement votre testbench (le fichier qui va tester votre design) .

Ajouter les Signaux au Waveform : Après avoir lancé la simulation, une nouvelle fenêtre sim apparaît. Faites un clic droit sur votre testbench et sélectionnez Add Wave ou Add to Wave . Cela ouvre la fenêtre Wave qui affichera les chronogrammes de vos signaux.

Forcer les Entrées et Exécuter : Dans la fenêtre Wave, vous pouvez forcer les signaux d'entrée (par exemple, un signal d'horloge) via la commande force ou en cliquant droit sur un signal et en choisissant Force . Ensuite, réglez la durée de simulation (par exemple 1000 ns) et cliquez sur le bouton Run pour voir l'évolution des signaux .
