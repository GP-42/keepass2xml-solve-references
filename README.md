# Solve References in KeePass2 XML export file
Resolves the references in a Keepass2XML export file

Call the script: $ python solve-references.py /path/to/keepass2.xml

Thanks for the great job, [Lukas](https://github.com/lsgd)!   
Without your work I'd have had a harder job implementing my solution.

I made 3 major changes to fit my personal use case:
1. Python3 didn't properly execute the existing Hex to Base64 conversion.
2. Empty Value tags also have to be copied as referenced value.
3. All references have to be followed, including the references to references.

The code can probably be tidied up.   
I currently don't have time to do this, but be my guest to perform a pull request and get your hands dirty.