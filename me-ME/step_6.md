## Povećavanje težine igre

Napravimo da igra postaje sve teža što duže igrač uspijeva da preživi, tako što ćemo polako smanjivati vremenski razmak između pojavljivanja tačaka.

+ Kreiraj novu promjenljivu i nazovi je `razmak`{:class="blockdata"}.

+ Na svojoj pozornici kreiraj novu skriptu koja postavlja razmak na visok broj, a zatim polako smanjuje vrijeme razmaka.
    
    ```blocks
        when flag clicked
        set [razmak v] to (8)
        repeat until < (razmak) = (2)>
            wait (10) secs
            change [razmak v] by (-0.5)
        end
    ```
    
    Primijetićeš da je ovo veoma slično načinu na koji funkcioniše odbrojavanje vremena!

+ Na kraju, promjenljivu `razmak`{:class="blockdata"} možeš da koristiš u skriptama crvene, žute i plave tačke. Ukloni kôd koji čeka slučajan broj sekundi za kreiranje novog klona i zamijeni ga svojom novom promjenljivom `razmak`{:class="blockdata"}:
    
    ```blocks
        wait (razmak) secs
    ```

+ Isprobaj svoju novu promjenljivu `razmak`{:class="blockdata"} i provjeri da li se vremenski razmak između tačaka polako smanjuje. Da li ovo funkcioniše za sve 3 obojene tačke? Možeš li da vidiš da se vrijednost promjenljive `razmak`{:class="blockdata"} smanjuje?