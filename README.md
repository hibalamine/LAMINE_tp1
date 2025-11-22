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
    tant que b=/0
    a<--b
    b<--r
    fin tant que 
    ecrire("le pgcd(a,b)est")
fin
    2)
ALGORITHME pgcd
  VAR:a,b,r
  fonction pgcd(a,b) 
  si b=0 alors
  retourner a
  sinon 
  retourner pgcd(b,a mod b)
  fin si 
  fin fonction
DEBUT
  ecrire("donner deux nombres")
  lire(a,b)
  ecrire("le pgcd (a,b)est")
     exercice 4 
     1)
ALGORITHME les_diviseurs_d_un_nombre
  VAR:n:ENTIER
DEBUT
  pour i de 1 à n 
  si n modi =0 alors 
  ecrire("i")
  fin si 
 fin pour
fin
     2)
ALGORITHME les_diviseurs_d_un_nombre
   VAR:n:ENTIER
DEBUT
   pour i de 1 à racineCarrée(n)
    si (n mod i=0)alors 
    ecrire (i)
    si i =/ n/i alors 
     ecrire n/i
    fin si 
   fin si 
  fin pour
fin
      exercice5
ALGORITHME deviner_entre_1_et_100
    VAR:n:ENTIER
   nombreSecret<-- aleatoire(1,100) 
   tentatives<--0
   MaxTentatives<--5
   tant que (MaxTentatives)
    lire(devine)
    tentatives<--tentatives+1
   si(devine=nombreSecret)alors
   ecrire("félicitations,vous avez deviné")
  sinon
  si(devine>nombreSecret)alors
   ecrire("trop grand")
   sinon
    ecrire("trop petit")
   fin si 
  fin tant que
  si(tentatives=MaxTentatives)et(devine=/nombreSecret)alors
  ecrire("le nombre correct est",nombreSecret)
 fin si 
fin
       exercice 6
ALGORITHME triangle_de_floyd
    VAR:nombre de lignes n: ENTIER
DEBUT
   ligne<--1
   compteur<--1
    tant que (ligne<=n)
    pour i de 1 à ligne
     ecrire("compteur")
   compteur<--compteur+1
   fin pour
    ecrire("nouvelle ligne")
   ligne<--ligne+1
  fin tant que 
fin
       exercice 7
     1)
ALGORITHME la_somme_des_entiers_de_1_à_n
   VAR:n,somme:ENTIER
DEBUT
  somme<--0
   pour i de 1 à n
  somme=somme+i
  fin pour
 ecrire("somme est",somme)
fin
      2)
ALGORITHME la_somme_des_entiers_de_1_à_n
     VAR:n,somme:ENTIER
   fonction somme(n)
    si n=1 alors
     retourner 1
    sinon
     retourner n+somme(n-1)
    fin si 
   fin fonction
DEBUT
 ecrire("somme est",somme)
fin


     