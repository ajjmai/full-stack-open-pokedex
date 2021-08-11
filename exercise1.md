# Exercise 11.1

My programming language of choice is Kotlin

## Linting, testing, building

Based on Google search, the two most common linters for Kotlin seem to be [ktlint](https://ktlint.github.io/) and [detekt](https://github.com/detekt/detekt). I have some experience using detekt and have found it a very useful tool. Intelli J IDEA has some built-in features for linting and formatting Kotlin.

Testing in Kotlin is quite similar to testing in Java. Kotlin has a [test library](https://kotlinlang.org/api/latest/kotlin.test/) that provides annotations to mark test functions and a set of utility functions for assertions. Also, JUnit can be used with Kotlin.

Gradle is a good choice for [a build tool for Kotlin](https://kotlinlang.org/docs/kotlin-and-ci.html). Other alternatives are, for instance, Ant and Maven.

## CI alternatives

One CI alternative for Jenkins and Github Actions mentioned in [Kotlin's documentation](https://kotlinlang.org/docs/kotlin-and-ci.html) is [TeamCity](https://www.jetbrains.com/teamcity/). It has been developed by the same company that developed Kotlin, JetBrains.

Gitlab and Gitlab's built-in CI pipeline is, of course, another alternative to Github and Github Actions.

## Hosting

JetBrain's TeamCity is available both as [cloud-based and self-hosted runners](https://www.jetbrains.com/teamcity/cloud/).

Some factors to consider when decising between self-hosting and cloud-based environment are scalability, cost and security.

Cloud-based environment is easy to set up and it is quickly scalable. It is often the best choice for small projects and one can usually set up a small pipeline for free. However, for bigger projects the cost can go up quickly when the amount of users and used runner minutes grow.

For big projects, a self-hosted environment might be a feasible alternative. It is often a must for high security projects. A down side with a self-hosted environment is that one has to manage all the infrastructure by one self, so it is not a good alternative when resources are low.
