### Contribute/Review Buttons v1
[![Contribute](http://codenvy.github.io/plugin-contribution/contribute-blue.svg)](http://a4.codenvy-dev.com/f?id=4m27r6nxed7bkhby)
[![Review](http://rawgit.com/sunix/90938b043d282fcd728c/raw/09c1878db322b335768568fd505277cbe8cfcb5d/review.svg)](http://a4.codenvy-dev.com/f?id=4m27r6nxed7bkhby)
### Contribute/Review Buttons v2
[![Contribute](http://rawgit.com/sunix/99c0da57ec96147bfd73/raw/e3eb038a56f7b9ed635eb06f551ccb225bbf50a9/codenvy-contribute-2.svg)](http://a4.codenvy-dev.com/f?id=4m27r6nxed7bkhby)
[![Review](http://rawgit.com/sunix/90938b043d282fcd728c/raw/9031bf6714c402e9f30626aa5f51560ed578cbff/review.svg)](http://a4.codenvy-dev.com/f?id=4m27r6nxed7bkhby)


# Codenvy Contribution Sample


A simple Hello World JAR. This project is a sandbox project for testing the contribution workflow plugin for Codenvy Eclipse Che: https://github.com/codenvy/plugin-contribution

For contributing to this project and test the contribute workflow, hit the contribute button provided at the top of the README. You'll be ready in a one-click operation

The buttons below are factory URLs generated with Codenvy CLI

## Generate your own contribution button for your test Codenvy/Eclipse Che server

Given that your are testing on a dev instance: http://dev.box.com

- Clone and build the [CLI project](https://github.com/codenvy/cli) in your workspace

        git clone git@github.com:codenvy/cli.git
        cd cli
        mvn clean install

- (optional) You can add your project to the PATH environment variable, for instance in my ~/.bashrc:

        export PATH=/home/user/path/to/cli:$PATH

- Anywhere, get our `factory.json` file that contains the right metadata

        wget https://raw.githubusercontent.com/codenvy/factories/factory-2.0/contribution-workflow/factory.json

- login to your Codenvy test serveur and create the factory

        codenvy remote add dev http://dev.box.com
        codenvy login --remote dev
        codenvy create-factory --remote dev factory.json

Done :)
