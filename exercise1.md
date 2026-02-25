My hypothetical project is a web development project. My team is responsible for building the back end for the application and they are using Java. 

Each developer run locally Checkstyle plugins in their IDE to ensure their code conforms to agreed coding standards set by the team. Naturally Checkstyle is also used in the CI. 

For testing in CI, application team uses several testing tools in the pipeline. Unit tests are ran using JUnit which is the most common unit test framework for Java. OWASP Dependency check is used to detect publicly disclosed vulnerabilities from libraries that are used in the project. Team also utilizes JMeter to constantly monitor performance of the endpoints. Any major degradation of performance will alert the team. Finally both front-end and back-end teams use playwright to E2E-test the application. 

As the technology stack in the project  is quite standard, team decided to use cloud based CI/CD tools. This will offload some of the responsibility and duties for maintaining the infra and software tools and help the team to concentrate what brings value to the company.

The team is not fond of Jenkins or Github because they are too mainstream technologies. The Company has not made any decisive decisions about where to run software anyways. Therefore the team has researched different options before hand on how to build CI/CD pipeline  for the application. For cloud based solutions, e.g. Amazon and Google Cloud, the team can use the vendor specific CI/CD platforms like Cloud Build in Google Cloud or AWS CodePipeline and CodeBuild. For Cloud agnostic solutions team could use CircleCI.
