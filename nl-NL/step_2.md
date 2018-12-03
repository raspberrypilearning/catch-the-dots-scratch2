## Een controller maken

We beginnen met het maken van een controller die wordt gebruikt om stippen te verzamelen.

+ Open het Scratch-project 'Vang de stippen' online op <a href="http://jumpto.cc/dots-go" target="_blank">jumpto.cc/dots-go</a> of download het vanaf <a href="http://jumpto.cc/dots-get" target="_blank">jumpto.cc/dots-get</a> en open het als je de offline-editor gebruikt.
    
    Je zou een controllersprite moeten zien:
    
    ![screenshot](images/dots-controller.png)

+ Draai de controller naar rechts als je op de rechterpijltoets drukt:
    
```blocks
wanneer groene vlag wordt aangeklikt
herhaal 
  als <key [right arrow v] pressed?> dan 
    draai (3) graden naar rechts
  end
end
```

+ Test je controller - hij zou naar rechts moeten draaien.