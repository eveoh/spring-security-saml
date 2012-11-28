Just a small fork to be able to make non-snapshot releases that play nicely with Maven.

To create release tags in your local git repo:

    mvn release:prepare

To perform the release while skipping tests (bad bad bad, but 1 of the tests may sometimes fail on local cacerts):

    mvn -Darguments="-Dmaven.test.skip=true" release:perform

