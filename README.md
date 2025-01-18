# MakeCode Skill Map

Github-hosted skill maps are loaded in the same manner as tutorials, with a URL fragment
formatted as follows:

`https://arcade.makecode.com/skillmap#github:[organization name]/[repository name]/[markdown file name]`

- Ex: https://arcade.makecode.com/skillmap#github:okanagan-code-academy/cargo-hauler-skillmap/skillmap.md

## Syntax

The skill map definition can be found in the `skillmap.md` file. Metadata about the skill
map itself can be found under the top-level heading:

- `id`: The string after the heading (eg `# sample`). Cannot contain spaces.
- `name`: The title of your skill map. This will be displayed in the banner on the page.
- `description`: A description of the map contents. This is also shown in the banner.
- `infoUrl` (optional): A URL to a page with additional educator information

### Learning Paths

A skill map consists of one or more "paths", each path being an ordered sequence of activities.
The first activity in each path is unlocked, and completing an activity unlocks the next one.

A learning path is defined by a level two heading (`##`) has has the following properties:

- `id`: The string after the heading (eg `## interface`). Must be unique within this skill map.
- `name`: The title of the path, displayed above the linked activities.
- `description`: Additional details (not currently displayed).
- `completionUrl`: URL to a certificate, displayed when a user has completed the entire path.

### Activities

Each learning path has multiple activities, defined by level three headings (`###`). Currently,
an "activity" is simply a MakeCode tutorial, and has the following properties:

- `id`: The string after the heading (eg `### space-activity1`). Must be unique within this skill map.
- `name`: The title of the activity. Displayed on the activity card.
- `type`: The type of activity. Must be `tutorial` currently.
- `description`: Details about the activity, displayed on the back of the card.
- `tags`: Descriptive tags displayed on the bottom of the activity card.
- `url`: Link to the tutorial. See the [MakeCode Tutorial Documentation](https://makecode.com/writing-docs/user-tutorials) for details on tutorial authoring and link formatting.
- `imageUrl`: URL for the image displayed on the front of the activity card.
