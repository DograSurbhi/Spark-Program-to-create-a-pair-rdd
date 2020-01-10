# Spark-Program-to-create-a-pair-rdd
 Download the file data-00007-of-00010.gz from this archive and extract it. 
 We want to create an RDD of the form (<URL1>,< URL2>) where URL1 is the URL of the page and URL2 is the URL of a page mentioned /linked to by  URL1. 
 
For example, if have the following record in wikilinks: URL ftp://217.219.170.14/Computer%20Group/sattari/word  MENTION vacuum tube 421 http://en.wikipedia.org/wiki/Vacuum_tube    MENTION vacuum tubes 10838 http://en.wikipedia.org/wiki/Vacuum_tube    MENTION electron gun 598 http://en.wikipedia.org/wiki/Electron_gun 

Then we want to create a pair rdd with the following elements:   
 (ftp://217.219.170.14/Computer%20Group/sattari/word, http://en.wikipedia.org/wiki/Vacuum_tube) (ftp://217.219.170.14/Computer%20Group/sattari/word, http://en.wikipedia.org/wiki/Vacuum_tube) (ftp://217.219.170.14/Computer%20Group/sattari/word, http://en.wikipedia.org/wiki/Electron_gun )
