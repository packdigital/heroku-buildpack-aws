Heroku buildpack for the AWS CLI
================================

This is a [Heroku buildpack](http://devcenter.heroku.com/articles/buildpacks)
that allows one to run AWS CLI in a dyno alongside application code.

Usage
-----

Example usage:

    $ heroku buildpacks:add heroku-community/awscli

    $ heroku config:add AWS_ACCESS_KEY_ID=<aws-access-key>
    $ heroku config:add AWS_SECRET_ACCESS_KEY=<aws-secret-access-key>
    $ heroku config:add AWS_DEFAULT_REGION=<default-aws-region>


````
curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"
unzip awscliv2.zip
sudo ./aws/install --install-dir aws-cli
````