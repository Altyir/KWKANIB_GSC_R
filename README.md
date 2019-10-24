# KWKANIB_GSC_R
With this R code, GSC data can be analyzed quickly and easily. 
CTR curve
Click curve
Weighting of one keyword per URL
Potentialle based on Impression



# Set Up R
1 Download R from here: https://cran.r-project.org/

2.download R-Studio from here: https://rstudio.com/ -> Uses the Free Version. You don't need anything else. 


Very important! Install first R and then R-Studio. R-Studio needs R to be installed!

# Set up the Code

1. Install all libraries in the console
	The code works as follows: install.packages("tidyverse") -> Each library must be installed for it to work!

2. Execute the code at the beginning only up to line 11. 
   After that a window will open where you have to allow access to your search console. 
   You will also get a token that you have to insert into the console.
   
If you have successfully completed step 2 you can run the whole code. Press str+a and then strg+enter once.


# Important side note for Windows
If you specify your location in line 105, always use two \, otherwise R cannot execute the command.

# Use in Excel
1. First convert the file (if needed) to an XLSX format.
   If you do not do this and create pivots in the CSV file, this will not be saved!
   
2. The following pivot filters can be used for the first step:

Row: positionRound Value: CTRmean -> Personal click-curve & CTR

Row: page+query ODER query+page Value: page(count)+clickP -> Click-percent calculation: Queries

Row: query+page Value: page(count) -> Keyword cannibalization

Row:  page+query OR query+page Value: per(sum) -> Click-percent calculation: URLs

Row:  page+query Value: positionRound(sum)+ctr(sum)+CTRmean(sum)+lower(sum)+upper(sum) -> Current CTR Limits




# KWKANIB_GSC_R

Mit diesem R Code lassen sich GSC-Daten schnell und einfach analysieren. 
CTR-Curve
Click-Curve
Gewichtung eines Keywords pro URL
Potenzialle basierend der Impression

# Set Up R
1 Download R hier: https://cran.r-project.org/

2.Download R-Studio hier: https://rstudio.com/ -> Nutzt die Free-Version. Alles andere wird nicht benötigt. 


Wichtig! Installiert zuerst R und erst danach R-Studio. R-Studio kann nicht installiert werden, sollte R nicht auf eurem Computer sein.

# Set up Code

1. Installiert alle bentötigten Libraries in der Console
	Der Code hierzu sieht wie folgt aus: install.packages("tidyverse") -> Jede Library muss installiert werden um sie zu nutzen.

2. Startet den Code beim ersten Mal nur bis Zeile 11. 
   Danach öffnet sich euer Browser und GSC fragt euch, ob ihr den Zugriff bestätigen wollt. 
   Nachdem ihr dies bestätigt habt, erhaltet ihr einen TOken den ihr wiederum in der Console einfügen müsst.
   
Wenn ihr Schritt 2 erfolgreich durchgeführt habt, könnt ihr den gesamten Code laufen lassen. Die Shortkeys hierfür sind str+a und dann str+enter.


# Wichtig für Windows-Nutzer
Achtet dabei in Zeile 105 euren Speicherpfad immer mit doppelten \ anzugeben, da ansonsten R nicht ausgeführt werden kann.

# Nutzung in Excel
1. Wandelt (falls benötigt) die Datei zunächst in ein XLSX-Format um.
   Solltet ihr dies nicht tun und in der CSV-Datei Pivots erstellen werden dies nicht abgespeichert!
   
2. Für den ersten Schritt können folgende Pivot-Filter eingesetzt werden:

Row: positionRound Value: CTRmean -> Personal click-curve & CTR

Row: page+query ODER query+page Value: page(count)+clickP -> Click-percent calculation: Queries

Row: query+page Value: page(count) -> Keyword cannibalization

Row:  page+query OR query+page Value: per(sum) -> Click-percent calculation: URLs

Row:  page+query Value: positionRound(sum)+ctr(sum)+CTRmean(sum)+lower(sum)+upper(sum) -> Current CTR Limits





