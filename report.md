Uživatel student měl povoleno bez hesla spouštět program zip jako uživatel spravce.
Program zip umožňuje číst soubory dostupné cílovému uživateli, což vedlo k přečtení souboru s vlajkou.
Nápravou je odebrání NOPASSWD sudo práv nebo striktní omezení povolených příkazů dle principu minimálních privilegií.
