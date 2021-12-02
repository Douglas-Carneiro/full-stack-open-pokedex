# Answer for exercise 11.1
## Linting ##
For linting, the tool of choice will be clj-kondo, since it is the most popular lint tool for Clojure with very active development, good documentation, and can be easily integrated with GitHub actions which is the tool the team is currently using for CI.

## Testing ##
Clojure provides a test API called clojure.test, this API provides all the basic and advanced set of functions for testing Clojure code, clojure.test is very complete with a good documentation, besides these features, it is possible to make some customizations to support some edge case the might want to test in the future.

## Building ##
We will use Leiningen as the building tool since this is a mature technology that fulfills all our needs for the build process, besides it offers declarative configuration and automation which will also help enormously with the packaging and testing tasks.

## Other CI Tools ##
After some search in Google I was able to find some other interesting CI tools, here is a list and a brief description:

### Circle CI ###
CircleCI is CI Tool that gracefully pairs with Github, one of the most popular version control system cloud hosting tools. CircleCi is one of the most flexible CI Tools in that it supports a matrix of version control systems, container systems, and delivery mechanisms. CircleCi can be hosted on-premise or used through a cloud offering. Source: https://www.atlassian.com/continuous-delivery/continuous-integration/tools 

### Team City ###
TeamCity is a powerful commercial CI solution that can be used for free during the first hundred build configurations. With TeamCity, you can run parallel builds at the same time, mark your builds and identify the hung ones. TeamCity is easy to install and its interface is really user-friendly. You’ll also love its community and professional support. Source: https://bitbar.com/blog/top-continuous-integration-tools-for-devops/

## Self-hosted or a cloud-based environment? ##
This setup is best suited for a cloud environment, with a possibility to transition for a self-hosted environment seamlessly. The team is small, we initially will not handle sensitive information, so our efforts cannot be wasted configuring a complex CI tool like Jenkins. In the future, if we see the need, we can transition to a self-hosted environment. Since GitHub Actions supports both types of environments this will be the CI tool of our choice.

Link to repository with solutions for exercises 11.21 & 11.22: https://github.com/Douglas-Carneiro/fullstack-bloglist