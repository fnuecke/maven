# maven

Static Maven repository via GitHub Pages at https://fnuecke.github.io/maven. Used for stuff I don't want to publish to
e.g. Maven Central, but is still nice to have available as a Maven-like dependency.

Reference as any regular maven repo, just make sure to filter for what you'll actually use to keep resolution fast.

```kotlin
exclusiveContent {
    forRepository { maven("https://fnuecke.github.io/maven") }
    filter { includeModule("li.cil.sedna", "sedna-buildroot") }
}
```
