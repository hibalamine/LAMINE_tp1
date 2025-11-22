# LAMINE_tp1
Mon premier projet
tp1 
nom:Lamine
prénom:Hiba
exercice 1
ALGORITHME code_pin_de_carte_sim
   VAR code pin:chaine de caractere
   CONST PIN_CORRECT="1234"= chaine de caractere 
DEBUT
    tentatives<--0
    MAXtentatives<-- 3
    tant que (MAXtentatives)faire
    ecrire("entrer le code PIN")
    lire(code PIN)
    si(code PIN=PIN_CORRECT)alors
    ecrire("code correct,accès autorisé")
    sinon
    tentatives<--tentatives+1
    ecrire("code incorrect,essaie encore")
    fin si 
    fin tant que 
    si (tentatives=MAXtentatives)alors
    ecrire("carte bloquée après 3 erreurs")
    fin si 
fin 
    exercice 2
ALGORITHME changement_des_valeurs_de_deux_variables
    VAR A,B,TEMPS
DEBUT
    ecrire("avant échange:","A=",A,"B=",B)  
fin
    exercice3
    1)
ALGORITHME pgcd
    VAR:a,b,r
DEBUT
    r<--a mod b
    tant que b