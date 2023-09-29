# Publish npm package workflow

This workflow will publish a npm package when a version tag is pushed.

## How to use

1. Copy the workflow file into your project (e.g. `.github/workflows/publish.yml`):
2. Commit and push the workflow file to your repository
3. Create a new release with a version tag (e.g. `v1.0.0`) with `git tag 'v1.0.0'` and push it to your repository with `git push --tags`
4. The workflow will run and publish the package to npm

:warning: **The new version take the tag version so becarfule the new version tag must be higher than the last published version. Otherwise the workflow will fail.** :warning:

## Configuration

Add the following secrets to your repository's secrets:

- `NPM_TOKEN`: A npm token with publish rights

## Used tools

[![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=github-actions&logoColor=white)](https://github.com/features/actions)

## Credits

- Author - [**Théo Gillet**](https://portfolio.theogillet.fr/)
