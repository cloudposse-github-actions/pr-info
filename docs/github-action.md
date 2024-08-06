<!-- markdownlint-disable -->

## Inputs

| Name | Description | Default | Required |
|------|-------------|---------|----------|
| filterOutClosed | True, False, 1 or 0 if only open PRs should be returned. Defaults to false. | N/A | false |
| filterOutDraft | True, False, 1 or 0 if only non-draft PRs should be returned. Defaults to false. | N/A | false |
| github-token | The GitHub token used to create an authenticated client. | ${{ github.token }} | false |
| sha | Sha to get PR for. Defaults to current sha. | N/A | false |


## Outputs

| Name | Description |
|------|-------------|
| body | The PR Body if one was found. |
| closed\_at | The PR Closed timestamp if one was found. |
| created\_at | The PR Created timestamp if one was found. |
| found | The outcome if a PR has been found. If so, the other outputs are set. |
| json | The whole PR object if one was found. |
| labels | The PR Labels if any was found. |
| merged\_at | The PR Merged timestamp if one was found. |
| number | The PR number if one was found. |
| title | The PR Title if one was found. |
| url | The PR Url if one was found. |
<!-- markdownlint-restore -->
