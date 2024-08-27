# My Github Search - An Alfred Workflow
Search all of your personal, starred, and organization repos in [Alfred](https://www.alfredapp.com/), a powerful MacOS launcher application. It uses the [GitHub REST API Endpoints](https://docs.github.com/en/rest/repos?apiVersion=2022-11-28).

Download from [releases](https://github.com/albertcai101/alfred-my-github-search-workflow/releases). Coming soon on the Alfred Workflow Gallery.
Then, follow the [setup guide](#setup).

![CleanShot 2024-08-27 at 00 52 15@2x](https://github.com/user-attachments/assets/fd329881-f042-4b21-b330-dee54d36257f)

## Dependencies
Alfred 5 with [PowerPack](https://www.alfredapp.com/powerpack/).

`jq`, which you can download at [their site](https://jqlang.github.io/jq/download/).

Nothing else, everything is in a single bash script :)

## Usage
`ghs {query}` will give you a list of all your personal, starred, and organization GitHub repositories. `⏎` on a selected result will open the repository in your default browser.

## Setup
After installing the Alfred workflow (download under Releases), click Configure Workflow... in Alfred. In the username text field, enter your GitHub username. 
In the token text field, generate a "Personal access token" at https://github.com/settings/tokens. You will need to check the following scopes:
- read:org
- repo
- user

![CleanShot 2024-08-27 at 00 46 56@2x](https://github.com/user-attachments/assets/f581332d-1ecb-4540-8fa3-0e6a9c02ed5c)
Note that I personally use a classic token so I can have no expiration date.

You can also customize the `ghs` command to any command of your choice in the same pane.
