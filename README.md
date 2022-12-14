# inngest/action-deploy-functions

This action installs the Inngest CLI ([inngest/inngest](https://github.com/inngest/inngest)) on your Linux, Mac, or Windows runner in GitHub Actions, then builds and deploys all functions found in the given directory.

See also:

- [inngest/action-test-functions](https://github.com/inngest/action-test-functions)

## Usage

```yaml
steps:
  - uses: actions/checkout@v3
  - uses: inngest/action-deploy-functions@v1
    with:
      token: ${{ secrets.INNGEST_AUTH_TOKEN }}
      dir: ./functions
      prod: true
```

You can also provide a `version` input to specify the version of the Inngest CLI to use. See [inngest/setup-inngest](https://github.com/inngest/setup-inngset) for more info.
