# US defense contract awards (DoD daily announcements)

Every contract announcement the US Department of Defense has published in its daily 5 pm ET release since July 2014, as one CSV: `dod_contract_awards.csv`. About 41,000 awards, updated each weekday evening shortly after the release.

| column | meaning |
|---|---|
| releaseDate | date of the daily release (YYYY-MM-DD) |
| agency | branch or agency section of the release (ARMY, NAVY, AIR FORCE, DEFENSE LOGISTICS AGENCY, ...) |
| contractor | company named first in the paragraph |
| location | the rest of the "company, city, state" phrase |
| amount | the award amount in USD as announced (the first dollar figure) |
| contractNumbers | contract numbers in the paragraph, space-separated |
| smallBusiness | true when the paragraph says the awardee is a small business |
| url | the release on war.gov |

Source: [war.gov contract announcements](https://www.war.gov/News/Contracts/), a US government work in the public domain. Parsing is automated, so check figures against the linked release before relying on them.

The same data with full text, search and filters is available as an API at [pushbuild.com/apis](https://pushbuild.com/apis/). Open federal bids by state: [pushbuild/us-federal-open-bids](https://github.com/pushbuild/us-federal-open-bids).

License: CC0 1.0.
