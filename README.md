Add password checker script using Have I Been Pwned API

This commit adds a Python script that checks the security of passwords
against the Have I Been Pwned API. The script computes the SHA-1 hash of
each password, sends the first 5 characters of the hash to the API, and
checks for a match in the response. If a match is found, the script
prints the number of times the password has been exposed in data breaches.
If no match is found, it prints that the password is secure.

The script accepts passwords as command-line arguments and can be used
to quickly check the security of multiple passwords. It also includes
error handling for API requests and responses.
