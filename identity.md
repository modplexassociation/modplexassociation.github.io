# Identity and signatures

Identity is a complex problem in general. We're not going to go deep here.

To keep track of our membership, I am proposing a two part solution:
1. The establishing of a web-of-trust type system.
2. Registration of the keys thus generated into a simple identity management database.

## Web of trust

This will follow models proposed by the PGP project [1], and CAcert[2] among others to generate an extending web of mod authors who can self-identify in whatever way they prefer, but with cryptographic strength to the same identity.

Introductions to the web-of-trust will come from existing members of the web of trust. We will use a system of vouching for others.

This will allow mod authors to identify themselves in a cryptographically strong way to systems that know about the web of trust, through the use of standard code signing tools such as Java's keytool. 

Having done this, modplex will be able to assure that mods so signed have well identified authorship, and are unmodified.

## Registration

Submitting verification of a web-of-trust signed key, will allow verification of membership in our association.

This will allow access to mechanisms such as certification revocations and changes - important functions that typically need a modicum of central control.

## Web of trust introductions

Introductions are a form of verification of identity. I (cpw) know that LexManos is this particular discord or twitter or github user, and thus I will sign a key offered to me from any of those known channels.

The identity encoded in each member's certificate should be their github identity where possible, since that is a widespread and common identity.

We'll probably need to encode that in the certificate request somehow.


[1]: (https://en.wikipedia.org/wiki/Web_of_trust) Web of trust
[2]: (https://en.wikipedia.org/wiki/CAcert.org) CAcert.org