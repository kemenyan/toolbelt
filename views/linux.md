<p class="download">
    <code>curl -L <a href="http://cl.ly/h">http://cl.ly/h</a> | sudo bash</code>
</p>

### What is it?

The Heroku Toolbelt for Debian/Ubuntu will give you everything you need to get started using Heroku. The installer contains:

* A standalone version of the [heroku client](http://github.com/heroku/heroku)
* [Foreman](http://github.com/ddollar/foreman) for running your apps locally
* [Git](http://git-scm.com/) for revision control and pushing to Heroku

### Getting started

Once installed, you'll have access to the heroku command from your command shell. Log in using the email address and password you used when creating your Heroku account:

    $ heroku login
    Enter your Heroku credentials.
    Email: adam@example.com
    Password:
    Could not find an existing public key.
    Would you like to generate one? [Yn]
    Generating new SSH public key.
    Uploading ssh public key /Users/adam/.ssh/id_rsa.pub

You're now ready to create your first Heroku app:

    $ cd ~/myapp
    $ heroku create --stack cedar
    Creating stark-fog-398... done, stack is cedar
    http://stark-fog-398.herokuapp.com/ | git@heroku.com:stark-fog-398.git
    Git remote heroku added

### Staying up to date

To keep your heroku client updated, simply run `heroku update`

    $ heroku update
    -----> Updating to latest client... done

### Technical details

The `heroku` command line client will be installed into `/usr/local/heroku` and the executable will be symlinked as `/usr/bin/heroku`.