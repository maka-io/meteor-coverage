# Velocity-Coverage

This package uses [Istanbul](http://gotwarlost.github.io/istanbul/) to instrument your meteor app code and collect code coverage from all velocity test runs.

## Usage

mrt add velocity-coverage

You can now use velocity as usual and you'll get coverage reports placed in `<your app>/tests/.reports/coverage`

#### Example app

Checkout the velocity example app and add the coverage package to see a demo:

```bash
$ cd ~/tmp
$ git clone https://github.com/xolvio/velocity-example.git
$ cd velocity-example
$ mrt add velocity-coverage
```

Because support for the coverage feature is fully merged into Velocity yet, you'll need to use the feature/coverage branch in your smart.json as follows:

```
    "velocity": {
      "git": "https://github.com/xolvio/velocity",
      "branch": "feature/coverage"
    }
```

Then you can start the app:

```bash
$ mrt
```

You'll see the leaderboard example started on port 3000, and once the tests have completed, you'll see a coverage report at `velocity-example/tests/.reports/coverage/index.html`

