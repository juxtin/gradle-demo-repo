
1. Clone juxtin/github-dependency-extractor (my fork has the maven-publish plugin)
2. Run `./gradlew publishToMavenLocal` in that repo
3. Run `./gradlew build` in _this_ repo

```
FAILURE: Build failed with an exception.

* Where:
Settings file '/Users/holguinj/src/gradle-demo-repo/settings.gradle.kts' line: 21

* What went wrong:
An exception occurred applying plugin request [id: 'org.gradle.github.dependency.extractor', version: '0.0.1']
> Failed to apply plugin 'org.gradle.github.dependency.extractor'.
   > class org.gradle.initialization.DefaultSettings_Decorated cannot be cast to class org.gradle.api.invocation.Gradle (org.gradle.initialization.DefaultSettings_Decorated and org.gradle.api.invocation.Gradle are in unnamed module of loader org.gradle.internal.classloader.VisitableURLClassLoader @66a3ffec)

* Try:
> Run with --stacktrace option to get the stack trace.
> Run with --info or --debug option to get more log output.
> Run with --scan to get full insights.

* Get more help at https://help.gradle.org

BUILD FAILED in 576ms
```
