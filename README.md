# Prince Edward Island: law history in git

Part of [lexifina/global-law](https://github.com/lexifina/global-law), one git history for every country's law: this is the law of Prince Edward Island, Canada, which global-law reads at `canada/prince-edward-island/acts/`.

The law of Prince Edward Island as a git history: one file per provision, one commit per law on the day it took effect, and the law that made each change as the commit's author. `git blame` names the law behind every paragraph; `git log` lists every change; picking a date gives the text in force that day.

It follows the shared design of [lexifina/global-law](https://github.com/lexifina/global-law).

## What this repository holds

**Metadata only, no law text: the official legislation site of Prince Edward Island and the Legislative Assembly's bill records are not used in this record.** This repository holds only a handful of open facts about the province's legal system. To read a statute, go to [Prince Edward Island legislation](https://www.princeedwardisland.ca/en/legislation). Law text will be added once the official text can be used.

| Folder | Act | Versions | History |
| --- | --- | ---: | --- |
| `legal-system/` | Legal system facts from Wikidata (CC0) | 2 | The province's inception (28 June 1769), then the facts as Wikidata held them on 18 September 2026 |

## Source

The facts are from [Wikidata](https://www.wikidata.org/wiki/Q1978) (CC0). Nothing is copied from the province's own sites.

## Dates

The province's inception is dated by Wikidata's day-precision date; the other facts are dated by the latest revision of the Wikidata item (18 September 2026; retrieved 30 October 2026). They were not enacted on those dates. Commits are at noon, Prince Edward Island time (America/Halifax, Atlantic time with daylight saving time).

## How it is checked

Every version is read back from git on the day it took effect and on the day before (`tools/check_repo.py`) and must match `corpus.json`; results are in `REPRODUCE.md`.

## What "author" means

The author of a commit is the law (or, for facts, the retrieval) that made the change, with an e-mail address that cannot exist (`<law key>@wikidata.org.invalid`). The committer is always Lexifina.

## Limits

No statute, regulation or bill is listed. Nothing here is an official record of the law of Prince Edward Island.
