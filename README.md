# hackathon-hc-card

Hackathon repository for creating specification files that harvesters can process.

## Structure

This repository is organized into folders for different types of specifications:

- `datasets/` - Dataset specifications
- `data-services/` - Data service definitions
- `events/` - Event specifications
- `concepts/` - Concept definitions
- `informationmodels/` - Information model specifications
- `services/` - Service specifications

## Contributing

1. Create a new branch for your team's work
2. Add your specification files in the appropriate folder
3. Ensure your specifications follow the expected format for harvesters
4. Commit and push your changes to your branch
5. Open a Pull Request to merge into `main`
6. Wait for team approval before merging


## Harvesting

1. Go to https://demo.fellesdatakatalog.digdir.no/publishing
2. Choose "Logg inn for å administrere høsting"
3. Choose "Logg inn via ID-porten"
4. Sign in with the provided demo-user (you'll need to set a new password on first login)
5. Refer to https://demo.fellesdatakatalog.digdir.no/publishing/about-harvesting if you're unfamiliar with the admin-portal.
6. Fill the form as per the documentation. "URL til datakilde" will be the URL to the RAW-format of the file you've added to this repository, i.e., https://raw.githubusercontent.com/fellesdatakatalog/hackathon-hc-card/refs/heads/main/services/tjenestekatalog-1 OR any other harvest endpoint where you've chosen to publish your file. Note that if you chose to not use this repo as harvest endpoint, you MUST include the organization number 555111098 OR the name of this repo somewhere in the URL i.e. the specification file name.
7. Save the data source and click harvest.
8. If the file is accepted, you'll be able to view it in our portal after a few minutes, depending on the datatype:
- Datasets: 10–15 minutes
- Concepts: 3–5 minutes
- Everything else: 1 minute
9. If the file isn't accepted, we'll likely have some log-ouput referring to why. We've set up a slack-channel that receives any harvest error related to this hackathon. Reach out to us if you want to be added to this channel.


## View harvested data in our portal

1. Go to https://demo.fellesdatakatalog.digdir.no/search-all?sortfield=FIRST_HARVESTED
2. Newly harvested data should be shown in this list
3. Use the search-bar, filter, or wait if you can't find your data in this list.