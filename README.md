# FileZilla XML Generator
This is a  PowerShell script that creates users programmatically to FileZilla Server by salting, hashing passwords and generate XML entries for them.

# Inputs
1. Usernames and passwords should be stored in CSV form, and should not have any spaces beside commas (Should be easy using Excel or Google Docs). 
2. Extra settings other than username and password should be written in another text file in Filezilla XML form. This part of text will be appended exactly the same, and will automatically be ended with </User> mark. So do not contain this mark in your file.

# Output
Generated XML for each user described in the provided CSV. Only the "User" sections are generated, so paste it inside the "Users" section in "FileZilla Server.xml", perform a reload, then it's done.
# Note

Filezilla Server does not require every option of a user to be provided, so neglect the unneeded can help the server apply its defaults.

And yes, f**k those indentations. The server will deal with it anyway.
