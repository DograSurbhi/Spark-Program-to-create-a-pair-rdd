# Spark-Program-to-create-a-pair-rdd
 Download the file data-00007-of-00010.gz from this archive and extract it. 
 We want to create an RDD of the form (<URL1>,< URL2>) where URL1 is the URL of the page and URL2 is the URL of a page mentioned /linked to by  URL1. 
 
For example, if have the following record in wikilinks: URL ftp://217.219.170.14/Computer%20Group/sattari/word  MENTION vacuum tube 421 http://en.wikipedia.org/wiki/Vacuum_tube    MENTION vacuum tubes 10838 http://en.wikipedia.org/wiki/Vacuum_tube    MENTION electron gun 598 http://en.wikipedia.org/wiki/Electron_gun 

Then we want to create a pair rdd with the following elements:   
 (ftp://217.219.170.14/Computer%20Group/sattari/word, http://en.wikipedia.org/wiki/Vacuum_tube) (ftp://217.219.170.14/Computer%20Group/sattari/word, http://en.wikipedia.org/wiki/Vacuum_tube) (ftp://217.219.170.14/Computer%20Group/sattari/word, http://en.wikipedia.org/wiki/Electron_gun )


Also, we need to find two things:
1. the number of times each URL has been mentioned by another URL and find 10 most frequently mentioned URLS. 
2. Find the number of symmetric URL pairs <URL1,URL2> such that  URL1 mentions URL2 and URL2 mentions URL1 . (Is there any such symmetric pairs in wikilinks?) 
