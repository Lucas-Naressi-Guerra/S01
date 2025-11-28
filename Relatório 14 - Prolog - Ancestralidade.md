progenitor(cronos, zeus).
progenitor(cronos, poseidon).
progenitor(cronos, hades).
progenitor(rhea, zeus).
progenitor(rhea, poseidon).
progenitor(rhea, hades).

dominio(zeus, ceu).
dominio(zeus, raio).
dominio(poseidon, mares).
dominio(poseidon, terremotos).
dominio(hades, submundo).

habitat(zeus, olimpo).
habitat(poseidon, olimpo).
habitat(hades, submundo).

deus_maior(Deus) :-
    habitat(Deus, olimpo),
    dominio(Deus, D1),
    dominio(Deus, D2),
    D1 \= D2.

ancestral(A, D) :-
    progenitor(A, D).

ancestral(A, D) :-
    progenitor(A, Z),
    ancestral(Z, D).
