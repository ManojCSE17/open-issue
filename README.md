# Github Issue Action

<p align="center">
  <a href="https://github.com/actions/javascript-action/actions"><img alt="javscript-action status" src="https://github.com/ManojCSE17/open-issue/workflows/units-test/badge.svg"></a>
</p>


This action opens a new github issue.

## Inputs

### `token`

**Required** Github Token.

### `title`

**Required** Issue title.

### `body`

Issue body.

### `assignees`

Issue assignees. Passed as a formatted multi-line string using the | character.

## Outputs

### `issue`

The issue object as a json string.

## Example usage of v1.0.0

```yaml
uses: ManojCSE17/open-issue@v1.0.0
with:
  token: ${{ secrets.GITHUB_TOKEN }}
  title: Some Issue Title
  body: Some Issue Body
  assignees: |
    ManojCSE17
```

## Example usage of latest version

```yaml
uses: ManojCSE17/open-issue@latest
with:
  token: ${{ secrets.GITHUB_TOKEN }}
  title: Some Issue Title
  body: Some Issue Body
  assignees: |
    ManojCSE17
```