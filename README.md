# MoveIt-CFML
MoveIt-HTTP is a CFML (Lucee and ColdFusion) library for interacting with the Progess MoveIT API for file transfer. 

While written primarily for ColdFusion implementations, this can easily be converted to fit whatever codebase you are working in since this is Java-based.
Attempting to use standard cfhttp to transfer files were not successful as the CF appends the full path to the filename, resulting in Error 2101 (Invalid Filename). MoveIt requires filename only, not the complete path.
By exposing the underlying Java http protocol, these functions strip the full path from the filename.
