NAME
====

**card-sign** -- sign a Card

SYNOPSIS
========

**virgil card-sign** \[-o *file*\] -s *file* -b *file* -k *file* \[--\]
\[--version\] \[-h\]

DESCRIPTION
===========

Sign a Card. You are building a model of trust by signing the Card

OPTIONS
=======

    -o *file*,  --out *file*
     Card Sign. If omitted, stdout is used

    -s *file*,  --signer *file*
     (required)  Signer's Card

    -b *file*,  --to-be-signed *file*
     (required)  Card to be signed

    -k *file*,  --key *file*
     (required)  Signer's Private key

    --,  --ignore_rest
     Ignores the rest of the labeled arguments following this flag

    --version
     Displays version information and exits

    -h,  --help
     Displays usage information and exits

EXAMPLES
========

1.  Alice is signing Bob's Card:

    virgil card-sign -s alice.vcard -b bob.vcard -k alice/private.key

SEE ALSO
========

[`virgil(1)`]()  
[`unsign(1)`]()  
[`card-search(1)`]()