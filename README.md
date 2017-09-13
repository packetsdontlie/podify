# podify
A MacOS helper script to take a web page and speak it now or save it for later (aiff, mp3)

## Usage
* Will use your system default voice: `/usr/local/bin/podify -u http://example.com`   
* Will speak the site with the Samantha voice `/usr/local/bin/podify -u http://example.com -v Samantha`  
* Will speak the site quickly with the Samantha voice, adjusting -r changes speed `/usr/local/bin/podify -u http://example.com -v Samantha -r 300`  
* Will save as AIFF `/usr/local/bin/podify -u http://example.com -v Samantha -s /path/to/file`  
* Will save as MP3 with lame installed `/usr/local/bin/podify -u http://example.com -v Samantha -s /path/to/file -c yes`  
* Will list your voices installed  `/usr/local/bin/podify -l yes`  

## Notes
* Dependent on the voices you have installed for MacOS
* Requires `curl`
* Conversion to MP3 requires the installation of `lame` which you can do via a package manager like brew
* Each voice in MacOS has a slightly different cadence, you may need to experiment to find the best value for `-r`

## Voices

`plank:vault b$ podify -l yes`   
`Agnes               en_US    # Isn't it nice to have a computer that will talk to you?`   
`Albert              en_US    #  I have a frog in my throat. No, I mean a real frog!`   
`Alex                en_US    # Most people recognize me by my voice.`   
`Bad News            en_US    # The light you see at the end of the tunnel is the headlamp of a fast approaching train.`   
`Bahh                en_US    # Do not pull the wool over my eyes.`   
`Bells               en_US    # Time flies when you are having fun.`   
`Boing               en_US    # Spring has sprung, fall has fell, winter's here and it's colder than usual.`   
`Bruce               en_US    # I sure like being inside this fancy computer`   
`Bubbles             en_US    # Pull the plug! I'm drowning!`   
`Cellos              en_US    # Doo da doo da dum dee dee doodly doo dum dum dum doo da doo da doo da doo da doo da doo da doo`   
`Daniel              en_GB    # Hello, my name is Daniel. I am a British-English voice.`   
`Deranged            en_US    # I need to go on a really long vacation.`   
`Fred                en_US    # I sure like being inside this fancy computer`   
`Good News           en_US    # Congratulations you just won the sweepstakes and you don't have to pay income tax again.`   
`Hysterical          en_US    # Please stop tickling me!`   
`Junior              en_US    # My favorite food is pizza.`   
`Karen               en_AU    # Hello, my name is Karen. I am an Australian-English voice.`   
`Kathy               en_US    # Isn't it nice to have a computer that will talk to you?`   
`Moira               en_IE    # Hello, my name is Moira. I am an Irish-English voice.`   
`Pipe Organ          en_US    # We must rejoice in this morbid voice.`   
`Princess            en_US    # When I grow up I'm going to be a scientist.`   
`Ralph               en_US    # The sum of the squares of the legs of a right triangle is equal to the square of the hypotenuse.`   
`Samantha            en_US    # Hello, my name is Samantha. I am an American-English voice.`   
`Tessa               en_ZA    # Hello, my name is Tessa. I am a South African-English voice.`   
`Trinoids            en_US    # We cannot communicate with these carbon units.`   
`Veena               en_IN    # Hello, my name is Veena. I am an Indian-English voice.`   
`Vicki               en_US    # Isn't it nice to have a computer that will talk to you?`   
`Victoria            en_US    # Isn't it nice to have a computer that will talk to you?`   
`Whisper             en_US    # Pssssst, hey you, Yeah you, Who do ya think I'm talking to, the mouse?`   
`Zarvox              en_US    # That looks like a peaceful planet.`   

## Adding New Voices

System Preferences >> Accessibility >> Speech >> System Voice >> Customize >> {select additional voices}
