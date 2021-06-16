# Oh Dear Request Run Action

> An Action to trigger a new mixed-content or broken-links run in Oh Dear.

This Action provides an abstraction to trigger new runs in [Oh Dear](https://ohdear.app) through GitHub Actions. These runs can either check your site for [broken links or mixed content](https://ohdear.app/feature/broken-page-check).


## Usage

Add the following step to a Workflow of your choosing.

```yaml
- uses: stefanzweifel/oh-dear-request-run-action@v1
  with:
    oh_dear_token: ${{ secrets.OH_DEAR_TOKEN }}
    check_id: 1234
```

Create a new [API token](https://ohdear.app/user/api-tokens) and store it as a secret in your repository or organisation.

You can find the `check_id` at the bottom of the "Broken Links" or "Mixed Content" page for each of your site in [ohdear.app](https://ohdear.app/sites).

## Versioning

We use [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/stefanzweifel/oh-dear-request-run-action/tags).

We also provide major version tags to make it easier to always use the latest release of a major version. For example you can use `stefanzweifel/oh-dear-request-run-action@v1` to always use the latest release of the current major version.
(More information about this [here](https://help.github.com/en/actions/building-actions/about-actions#versioning-your-action).)

## Credits

* [Stefan Zweifel](https://github.com/stefanzweifel)
* [All Contributors](https://github.com/stefanzweifel/oh-dear-request-run-action/graphs/contributors)

## License

This project is licensed under the MIT License - see the [LICENSE](https://github.com/stefanzweifel/oh-dear-request-run-action/blob/main/LICENSE) file for details.
