# gradle-minimum

Minimum compatible versions of Gradle.

## Motivation

Make sure your toolchain is always compatible with Gradle. (as Gradle will drop older versions)

## Versions

- [`java`](version/java)

## Example

### GitHub Actions - Java

```yml
- run: echo "JAVA_VERSION=$(curl -L https://github.com/WaterLemons2k/gradle-minimum/raw/main/version/java)" >>"$GITHUB_ENV"
- uses: actions/setup-java@v4
  with:
    distribution: temurin
    java-version: ${{ env.JAVA_VERSION }}
```
