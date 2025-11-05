# Calcul Salariu

## Descriere
Acest proiect implementeaza o baza de date pentru gestionarea salariatilor, pontajului si calculului salariilor in functie de timpul efectiv lucrat, sectia/proiectul alocat, precum si retinerile datorate absentelor.

## Sistemul gestioneaza:

1. salariatii si datele lor personale
2. pontajul zilnic
3. proiectele si sectiile in care se desfasoara activitatea
4. calculul salariului in functie de orele lucrate
5. retinerile bazate pe absente
6. manopera la nivel de sectie
7. determinarea angajatilor cu salariile maxime/minime


## Obiective 

1. Crearea si instantierea bazei de date cu toate constrangerile de integritate
2. Calculul salariilor pe fiecare salariat
3. Calculul manoperei pe fiecare sectie
4. Determinarea muncitorilor cu cele mai mari / mici salarii
5. Calcularea retinerilor (nr_absente × tarif_ora)


## Structura bazei de date

## Tabele principale

1. Salariati
2. Pontaje
3. Retineri
4. Sectii
5. Sefi_departamente
6. Proiecte


## Relatii cheie

1. Angajatii sunt alocati proiectelor si sectiilor prin pontaje
2. Retinerile sunt asociate angajatilor
3. O sectie are un sef de departament
4. Proiectele au bugete proprii


## Constrangeri de integritate

1. Chei primare (PK)
2. Chei straine (FK)
3. CNP unic
4. SALARIU_ORA > 0
5. Durata si nr_ore ≥ 0
6. Nr_absente ≥ 0
7. Buget ≥ 0