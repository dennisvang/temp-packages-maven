Maven project based on [Maven getting-started guide][1].

Github packages workflow based on the template [maven-publish][4] from the github starter workflows. 
Also see [Github packages quickstart guide][2] and the example [publishing java packages with maven][3].

Configuration for publishing packages is handled by github's [`setup-java`][5] action, by creating a `settings.xml`.
Also see [working with the apache maven registry][6] and [Maven pom docs][8].

If using gpg, e.g. for publishing to maven central, the pom requires some additional config, as described [here][7].

[1]: https://maven.apache.org/guides/getting-started/index.html
[2]: https://docs.github.com/en/packages/quickstart
[3]: https://docs.github.com/en/actions/use-cases-and-examples/publishing-packages/publishing-java-packages-with-maven
[4]: https://github.com/actions/starter-workflows/blob/main/ci/maven-publish.yml
[5]: https://github.com/actions/setup-java/blob/main/docs/advanced-usage.md#Publishing-using-Apache-Maven
[6]: https://docs.github.com/en/packages/working-with-a-github-packages-registry/working-with-the-apache-maven-registry#publishing-a-package
[7]: https://github.com/actions/setup-java/blob/main/docs/advanced-usage.md#extra-setup-for-pomxml
[8]: https://maven.apache.org/pom.html#Distribution_Management
