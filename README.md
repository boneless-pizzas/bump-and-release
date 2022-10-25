# Bump and Release 

Re-usable workflow test for Node projects that can be referenced like so:

```
name: Bump Version and Release

on:
  pull_request:
    branches:
      - main
    types: [closed]

jobs:
  bump_and_release:
    uses: boneless-pizzas/bump-and-release/.github/workflows/bump-and-release.yml@main
    secrets: 
      BOT_TOKEN: ${{ secrets.BOT_TOKEN }}
```
