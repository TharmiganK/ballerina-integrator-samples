# Scatter Gather flow control with email

This example shows the usage of the scatter-gather control flow to aggregate data in parallel and return the result in JSON.

The example uses prepared data as input for two resources that should be aggregated. The data represents information about two contacts and has the following structure:

| Resource | firstname | surname | phone | email |
|---------|-----------|--------|-------|-------|
| contacts_1.csv | John |	Doe | 096548763 | john.doe@texasComp.com |
| contacts_2.csv | Jane |	Doe | 091558780 | jane.doe@texasComp.com |

The information about the contacts is aggregated to a JSON structure that represents data from both resources (contacts_1.csv and contacts_2.csv which are located in the resources directory). Then, the report is sent to an email address via the Google Gmail connector.
