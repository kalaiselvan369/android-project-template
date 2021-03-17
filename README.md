# Android Project Template
Android project template with inital setup before starting development.

## Git hooks
Having this setup ensures the code formating and branch name convention check before every commit.
[Link to file](pre-commit)

## Spotless plugin
Does code formatting check and provides the report. This is already automatted in pre commit hook.
[Ref: Spotless repository](https://github.com/diffplug/spotless)

### to check for errors, run
`./gradlew spotlessCheck`
### to fix errors, run
`./gradlew spotlessApply`

## Github workflows
Like anyother CI/CD tools and services, we can automate our unit tests and release builds to firebase distribution or playstore using 
this workflow available in the github. It uses few github actions for checking out repository in the github hosted server and other tools 
like fastlane for app distribution.

[Link to workflow](.github/workflows/main.yml)

## Fastlane
To automate the build releases to playstore/firebase distribution. Fastlane setup in this project is done via bundler as described in
the docs for better usage.

[Link to fastfile](fastlane/Fastfile)

[Ref: Fastlane](https://docs.fastlane.tools/getting-started/android/setup/)

