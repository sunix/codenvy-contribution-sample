### Contribution workflow
[![Contribute](https://rawgit.com/slemeur/4a900bb68300a2643679/raw/1ad2c6d784c92fc21886c765bc6315a1f2ee690c/codenvy-contribute.svg)](http://a4.codenvy-dev.com/f?id=86aany3cbz7q2583) a4 contribute workflow

[![Contribute](https://rawgit.com/slemeur/4a900bb68300a2643679/raw/1ad2c6d784c92fc21886c765bc6315a1f2ee690c/codenvy-contribute.svg)](http://nightly.codenvy-stg.com/f?id=yrtazdmruzya046n) nightly contribute workflow


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

qsdfqsdfqsdf
