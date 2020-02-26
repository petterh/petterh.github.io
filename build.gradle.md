# Understanding build.gradle

Messing with Android Studio build.gradle files have long been a matter of copying working code from Stack Overflow and tweaking it to fit. This usually entails a good deal of trial and error.

I've tried to build a conceptual model of how this-all works, and here are the results.

## The files

There are usually at least two `build.gradle` files: One for the overall project, and one for each module, of which there are typically at least one. The "master" file applies to all projects.

You may have additional files and include them using `apply`.

Then there is `settings.gradle` in the root, which includes modules as necessary. And properties &ndash; those are conceptually problem-free.

* A given task may result in many tasks, given multiple configurations or flavors
* What does "configure a project" mean? Configuration phase -> execution phase?

## Links

[Building Android apps](https://guides.gradle.org/building-android-apps/)
