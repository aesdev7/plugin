# In search for the optimal persistence mechanism

# A plug-in database (hosting apps projects) stored in a shelve. 
# Python modules : 
      - pickle       : 
      
      - shelve       :      Open the shelve file, and access it through a dictionary-like API.
                            Objects saved to the database are automatically pickled and saved 
                            One drawback of shelve is that when using the default interface there is no way to predict
                            which DBM format will be used: shelve selects one based on the libraries available on the
                            system where the database is created.
                                  
      - json         :      (frequently used for web-based applications.it integrates better with existing web service storage tools).
                            For web applications that work with data in JSON already, use of json (page 803) and dbm (page 408).
                            

      
      - DBM          :     Using dbm directly requires a little more work than using shelve because the DBM database keys and values must be
                           strings, and the objects will not be re-created automatically when the value is accessed in
                           the database.
                           
                           
                           Advantage of the DBM format : 
                                         >  Objects saved to the database are automatically pickled and saved.

# Data           :     
                        >       Data with no indexing or lookup ; 
                                                                        a simple flat file with serialized objects written one after the other. 
                        >       Data indexed looked-up          ;
                                                                        modules for storing key–value pairs in a simple database using one of the DBM
                                                                        format variants











                                                                        The most straightforward way to take advantage of the DBM format is to use shelve
(page 405). Open the shelve file, and access it through a dictionary-like API. Objects saved
to the database are automatically pickled and saved without any extra work by the caller.

      Convert objects into a format that can be transmitted or stored 
                   
      db   :      To preserv data for long-term use.

                  Task      :
                              1. Make an in-memory data object convertable to savable format that can be transmitted or stored.
                              2. how to store the data. A simple flat file with serialized objects written one after
                                 the other 
