# KnowMore-Your-Secondary-Brain
The project allows you to store all the information that you feel important on the internet at one place.

While researching any topic on the internet, people generally end up opening multiple tabs and curate information from various links that they find useful. However, retrieving the source of this curated information later is comparable to finding a needle in the haystack. 

KnowMore is designed to ease and expedite this task. While browsing on the internet, if the chrome extension for KnowMore is switched on, the user can simply select any text on a website and copy it. This text along with its source link is then saved into the database.  

With KnowMore search engine, the user can later retrieve the specific information along with its source link.

At its backend, KnowMore entails some aspects of Natural Language Processing and Distributed Computing. KnowMore uses MongoDB to store all the data. 

The search engine uses TF-IDF algorithm to retrieve documents matching the entered query. The architecture of this search-engine comprises of one database server, one master server and many slave servers (which can be dynamically added or removed).

When the user enters a query, the request is passed to the Master Server which determines the server (Slave server) on which the request should be executed. Once decided, the selected slave server communicates with the database server and fetches the relevant results.
