<!-- -*- mode: markdown; coding: utf-8 -*- -->
# Finnish Radio Amateur Callsigns

File [oh-callsigns.tsv](oh-callsigns.tsv) contains Finnish radio
amateur callsigns which are downloaded daily from
[Finnish Communications Regulatory Authority](https://www.viestintavirasto.fi/en/index.html).

The purpose of this repository is to provide historical data about
callsigns which is not available from the authority.

Maintainer: [Joel Lehtonen](https://github.com/zouppen/) / OH6EYA

## How to use

Just clone this repository and then `git pull` periodically
(e.g. in a cron job or systemd timer).

**NB!** Please do not use `fetch_from_ficora` unless you are hosting a mirror
yourself.

## File format

The first column contains the call sign. The second column contains status, which may be either:

* `VOIMAS`: Active call sign
* `KARENSSI`: On cooling period. This call sign becomes available
  after two years of inactivity.
  [source](https://www.viestintavirasto.fi/taajuudet/radioluvat/radioamatoorit.html#radiolupauusitaanviidenvuodenvalein)

Call signs on cooling period may contain an asterisk (such as
`OH*EEG`). That means the sign is reserved in all regions (0-9).

## License

All files except `oh-callsigns.tsv` are certainly public domain. The call
sign data is most likely public domain, but the data is sourced from
FICORA and I'm not a lawyer.
