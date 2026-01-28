Útok fungoval, protože uživatel student mohl spouštět program zip jako uživatel spravce bez hesla.
Parametr -TT umožňuje spuštění libovolného příkazu, což vedlo k eskalaci privilegií.
Administrátor by měl omezit sudo práva, zakázat nebezpečné parametry nebo nepovolovat zip v sudo.
