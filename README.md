# action-gradle-builder
Compiles Android Apps using gradle.
(doesn't support private repos)

# inputs
## Repo URL
This is the URL to the app's repo. 
Example:
```https://github.com/sounddrill31/UiBench.git```

If you want to clone a specific branch, just add `-b revision-name-or-id` at the end

Same way, if you want to pass any other arguments to git clone, add it at the end like `--depth=1`. Remember to use --depth=1 when dealing with AOSP-like repos with huge repo sizes and commit history


## Repo Path
If it is a simple git repo where the source files are available in the project root, just enter the repo name.

Example:
```UiBench```

If the files are elsewhere, you can specify the path here. 

## Gradle version
This is used to generate gradle wrapper files to use custom Gradle Versions.

*Ignored if gradlew files exist*
