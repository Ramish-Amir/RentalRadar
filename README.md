﻿# RentalRadar

**Concepts Used:**<br/>
1) Sorting (Merge Sort)
2) Ternary Search Trie
3) Hash Maps
4) Text Processing (JSoup, String Functions)
5) Memory Management (Caching)

**Flow of Execution of the Search Engine:**<br/>
1) Use of Java web crawler to crawl the web and recursively retreive around 1500 URLs from 3 different rental websites.<br/>
2) Each URL is parsed to a text file using JSoup. 
3) Stop words are removed from the Search String given by the user.
4) String is converted to token using Java String Tokenizer.
5) All URLs are indexed into a Hash Map.
6) TST is generated for each text file and frequency of keywords are extracted.
7) To implement page ranking, frequency of these words along with the URL index are stored in the Hash Map.
8) The page ranking Hash Map is sorted in decreasing order of frequency words.
9) Page ranking Hash Map is stored in memory to implement cache and drastically improve search time.
