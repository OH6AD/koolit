<!-- -*- mode: markdown; coding: utf-8 -*- -->
# Finnish Amateur Radio Callsigns

File [oh-callsigns.tsv](oh-callsigns.tsv) contains Finnish
amateur radio callsigns which are downloaded daily from
[Finnish Transport and Communications Agency](https://www.traficom.fi/en).

The purpose of this repository is to provide historical data about
callsigns which is not available from the authority. There are graphical
diagrams made from this data at [ham.may.fi](http://ham.may.fi/ohcounts/).

Maintainer: [Joel Lehtonen](https://github.com/zouppen/) / OH64K

## How to use

Just clone this repository and then `git pull` periodically
(e.g. in a cron job or systemd timer).

**NB!** You should do not use `fetch_from_ficora` unless you are hosting a mirror
yourself.

## File format

The first column contains the call sign. The second column contains the status information. See table below:

Key | Legend
--- | ---
`VOIMAS` | Active call sign
`KARENSSI` | On a grace period. This call sign becomes available after two years from expiry.
`VARAUS` | The call sign has been reserved for an applicant but not yet been issued.

Call signs on grace period may contain an asterisk (such as
`OH*EEG`). That means the sign is reserved in all regions (0-9).

## License

All files except `oh-callsigns.tsv` are certainly public domain. The call
sign data is most likely public domain, but the data is sourced from
Traficom and I'm not a lawyer.
