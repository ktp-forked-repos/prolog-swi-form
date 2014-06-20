prolog-swi-form
===============

Przykład obsługi formy z użyciem SWI-Prologu jako serwera HTTP.

Uruchomienie serwera na porcie 5000
------------------------------------

`$ ./start
`
Ctrl-C  (przerwanie programu i zatrzymanie serwera)

Uruchomienie serwera na dowolnym porcie
---------------------------------------

Przykład uruchomienia serwera na porcie 2000:

`$ swipl
Welcome to SWI-Prolog (Multi-threaded, 64 bits, Version 6.6.0)
Copyright (c) 1990-2013 University of Amsterdam, VU Amsterdam
SWI-Prolog comes with ABSOLUTELY NO WARRANTY. This is free software,
and you are welcome to redistribute it under certain conditions.
Please visit http://www.swi-prolog.org for details.

For help, use ?- help(Topic). or ?- apropos(Word).

?- [mainfile].
% ...
% mainfile compiled 0.17 sec, 4,221 clauses
true.

?- server(2000).
true.

?- TU MOŻNA DALEJ PROWADZIĆ DIALOG Z PROLOGIEM`

?- halt. % zakończenie pracy z PROLOGIEM i jednoczesne zatrzymanie serwera

Obejrzenie strony WWW
---------------------

Po uruchomieniu serwera należy w przeglądarce wpisać następujący adres (gdy port 5000):

		http://localhost:5000/form
