Test environment for debugging a Python memory problem. See
http://stackoverflow.com/questions/15350477/memory-leak-opening-files-128kb-in-python

Use a virtual environment to ensure some system site packages do not affect results:

    $ virtualenv venv
    $ source venv/bin/activate

To run the script that leaks memory:

    $ ./runtest debug_memory_leaks.py
    
To run the script that does not leak memory:

    $ ./runtest debug_memory_freed.py
