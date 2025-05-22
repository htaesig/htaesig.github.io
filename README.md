# HTA ESIG webpage
Rendered site available [here](https://htaesig.github.io/).

# Instructions for site maintainers

## Editing pages

- Landing page: ``index.html`` 
- Subpages: ``_pages/*.md``

## Adding new posts (``Communocations``)

1. Go to the ``_posts`` folder
2. Select ``Add File`` / ``Create new file`` in top right corner
3. Follow naming convention ``2024-10-02-xxx.md`` (i.e. year, month, date, your topic)
4. Follow markdown structure from old posts 

## Adding other file types (presentations etc)
- Upload to ``downloads``
- Follow same naming convention as ``_posts`` (i.e. year, month, date, your topic) to maximize traceability
- Include link in markdown with ``[Click here](/downloads/2025-04-09-april-2025-hta-esig-meeting-training-subteam.pdf)``

## Editing navigation bar
- ``_layouts/default.html``

## Editing subteam information
- ``_data/subteams.yml``

## Efficient workflow for ESIG (meeting slides+minutes in one go)
1. Utilize a markdown web rendering app such as https://typo.robino.dev/
2. Draft slides locally and paste into  web app and for presenting during meeting
3. Do minimal edits to get back to github markdown and repurpose slides as minutes

# Acknowledgments
Theme forked from [Reverie](https://github.com/amitmerchant1990/reverie/)

# License

MIT
