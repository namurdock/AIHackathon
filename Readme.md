# Overview

Working with Not For Profit organisations over the last 6 years I have found that due to the target audience of most of them utilising new technology is not something that comes easily due to a lot of the transactions still occurring offline via cash or cheque.

Finally with the introduction of the Document scanning AI models in the Power Platform these organisations can now leverage the power of AI to speed up processing of cheques that arrive through the post on a daily basis. Allowing the person sorting through the mailbag to scan and tag the cheques as they come in, tag them with the correct financial coding information and then save them in the Dataverse.

Then, using Chat GPT, have the system generate a thank you message to the donor taking into consideration why the donation was given and for what cause.

# Full solution features

- Model Driven App "Income Tracker" for the back office administration of data.
- Custom tables for Transactions, Transaction Types, Appeals and Projects to illustrate a possible financial coding model that could be integrated with Business Central Dimensions.
- Canvas App "The Postbook" for use by the "front of house" staff to record and tag incoming cheques.
- Custom Connector to connect to Chat GPT (due to region restrictions at time of development)
- Cloud Flow "Generate Thank you email" to utilise the custom chat GPT connector and generate a bespoke email thanking the donor for their support.
- MS Fabric Lakehouse for the entity changes in the system to be exported to for Power BI reporting
- MS Fabric Datamart to normalise the backend data model into a more user friendly dataset with predefined relationships
- Power BI report surfacing useful metric on income trends.

# Where to Next?

The upcoming release of CoPilot for Power BI should bring powerful reporting to the end users, making use of a clean dataset curated in MS Fabric Datamart.

The AI model for document scanning could be extended to help process Direct Debit Paper forms as well as Gift Aid declarations in the UK. Speeding up many areas where users have to manually transfer information from structured forms into the Dataverse.
