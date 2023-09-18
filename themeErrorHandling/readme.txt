--------------------
Theme Error Handling
--------------------
Hvis et tema får loadState=LOAD_ERROR, starter værktøjet en dialog-boks, der giver en mere brugerrettet besked, end den røde fejlmeddelelse, der er standard i Spatial Suite.


--------------------
INSTALLATION
--------------------

1:   Modulet ligges i ..\config\modules\custom\themeErrorHandling

1.a:  Tilføj følgende linie til modulfilen:

    <module name="themeErrorHandling" dir="custom/themeErrorHandling" permissionlevel="public"/>.

2: I toolet er der defineret nogle beskeder baseret på primaryendpointtype. De skal nok tilpasses til egne ønsker.
	Man kan også justere på maxDialogs, der forhindrer at der åbnes ubegrænsede antal samtidige dialogvinduer.

3:	Tilføj toolet til profil
	<tool ignore="not ModuleDefined('themeErrorHandling')" module="themeErrorHandling" name="themeErrorHandling_plugin"/>