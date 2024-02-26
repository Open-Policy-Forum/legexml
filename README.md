# legexml

## [WIP] XML standard for fully self-contained description of US state legislative instruments.
OPF uses XML at certain points in our backend. This repo is for documenting it, standardizing it, and making it available. Considering our schema from a standards-based POV and not just a problem-solving POV facilitates robustness and interoperability.  

For now, the repo is a scratchpad. Eventually it will hold our schema and the final product of refactoring our ad-hoc beta XML to match.

### Prior efforts in the space (-ish) we're aware of:
* [OASIS LegalDocumentML](https://www.oasis-open.org/committees/tc_home.php?wg_abbrev=legaldocml)
* [OpenCivicData (2014 archive link)](https://web.archive.org/web/20140707131451/https://opencivicdata.org/)
* [The State Decoded](https://github.com/statedecoded/statedecoded/releases/tag/1.0)
* [OpenStates API](https://docs.openstates.org/data/)
* [Legiscan API](https://legiscan.com/gaits/documentation/legiscan)


### Why are you doing this? Haven't you read [the XKCD comic about standards?](https://xkcd.com/927/)

Because nobody uses OASIS LDML, OpenCivicData and State Decoded are dead, and other people's APIs are neither yours nor free (beer/speech/often both). Internally at OPF we need a portable, offline, self-contained way to fully describe a bill, and we expect that sort of thing will be useful in many other contexts. You don't know what you've got 'til it's gone and you don't know what you've been missing 'til you've got it - well, now we've got it, and it turns out we've all been missing quite a lot! 

### Do it in JSON?????

No :)