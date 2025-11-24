# Github username data
Public data on GitHub username registrations of different lengths and combinations.

**_NOTES_**

_This project is just for fun, please DO NOT violate any official policy of the GitHub platform._

# Data file name rules

    element.length.gud

The element part can be only alphabets, only numbers, alphabets with dash(-), numbers with dash, or alphabets and numbers with dash.

Example:
```
alphabet.4.ghud
number.4.ghud
alphabet-.4.ghud
number-.4.ghud
alphabet-number.4.ghud
alphabet.5.ghud
alphabet.6.ghud
```

The suffix .ghud means GitHub username data.

# Data format

Only three columns, and the first one is a username string, the second one is the state:
- 0: registered
- 1: 404/BINGO
- 2: reserved
- 3: unknown 

The third one is the last check datetime in UTC/UNIX timestamp format. (WHY? Because GitHub users are free to change their usernames subject to the Platform's policies)

- Use one space as a delimiter.
- No table head. 

Example: 

```
username1 0 1763953750
username2 1 1763953750
username2 3 1763953750
```

# GitHub Policy

- GitHub enforces a username policy: <https://docs.github.com/en/site-policy/other-site-policies/github-username-policy>
- If your account namespace contains any public repositories that either include an action listed on GitHub Marketplace, or had >100 clones or >100 uses of GitHub Actions in the week before you rename the account, the old owner/repo name combination (OLD-OWNER/REPOSITORY-NAME) is permanently retired and cannot be reused.
- Packages and container images in GitHub Packages are transferred to the new namespace. Public container images with >5,000 downloads have the full former name permanently retired after a rename.
- Repository web links to existing repos continue to work (redirects) — this can take a few minutes. Command-line pushes to old remote URLs also continue to work.
- GitHub cannot create redirects for:
  - @mentions that used your old username
  - Links to gists that include your old username
- Verified commits using the previous GitHub-provided noreply email will lose their "Verified" status after a username change.
- Whether commits tied to a GitHub-provided private commit email are retained depends on the noreply address format. Commits using ID+USERNAME@users.noreply.github.com remain associated with your new username; older noreply formats without a numeric ID may not be associated after renaming.
- Username reference <https://docs.github.com/en/account-and-profile/reference/username-reference>
