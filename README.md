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
