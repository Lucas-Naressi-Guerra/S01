% Fatos de parentalidade
filho(zeus, cronos).
filho(zeus, reia).

filho(posseidon, cronos).
filho(posseidon, reia).

filho(hades, cronos).
filho(hades, reia).

% Domínios
dominio(zeus, ceu).
dominio(posseidon, mar).
dominio(hades, submundo).

divindade_olimpica(Deus) :-
    filho(Deus, cronos),
    dominio(Deus, Dominio),
    member(Dominio, [ceu, mar, submundo]).
