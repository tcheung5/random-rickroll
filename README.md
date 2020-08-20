# Random Rick-Roll

This action comments a gif of rick ashley when someone opens a new issue.

## Inputs

### `percentage`

**Required** How many people out of hundred should be rickrolled (set this to 100 if you want to rickroll everyone).

### `message`

**Optional** Comment message when not rickrolling (No comment would be made if not provided).

### `GITHUB_TOKEN`

**Required** Github token of the repository.


## Example usage



```
on:
  issues:
    types: [opened]

jobs:
  comment:
    runs-on: ubuntu-latest
    steps:
      - name: Rick Roll
        uses: TejasvOnly/random-rickroll@v1.0
        with:
          percentage: 100
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}'
```
