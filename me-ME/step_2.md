## Izrada kontrolera

Počnimo sa izradom kontrolera koji će se koristiti za sakupljanje tačaka.

+ Otvori Scratch projekat 'Catch the Dots' online na <a href="https://scratch.mit.edu/projects/240006242/#editor" target="_blank">scratch.mit.edu/projects/240006242/#editor</a> ili ga preuzmi sa <a href="http://github.com/raspberrypilearning/catch-the-dots-scratch2/raw/master/me-ME/resources/CatchTheDotsResources.sb2" target="_blank">jumpto.cc/dots-get</a>, a zatim otvori ako koristiš offline editor.
    
    Trebalo bi da vidiš lik (sprite) kontrolera:
    
    ![screenshot](images/dots-controller.png)

+ Okreni svoj kontroler udesno kada je pritisnut taster sa strelicom udesno:
    
    ```blocks
        when flag clicked
        forever
            if <key [right arrow v] pressed?> then
                turn right (3) degrees
            end
        end
    ```

+ Isprobaj svoj kontroler - trebalo bi da se vrti udesno.