## Install Node from the EPEL Repository
An alternative installation method uses the EPEL (Extra Packages for Enterprise Linux) repository that is available for CentOS and related distributions.
To gain access to the EPEL repo, you must modify the repo-list of your installation. Fortunately, we can reconfigure access to this repository by installing a package available in our current repos called epel-release.

1. sudo yum install epel-release

Now that you have access to the EPEL repository, you can install Node.js using your regular yum commands:

2. sudo yum install nodejs

Once again, you can check that the installation was successful by asking Node to return its version number:

node --version
v0.10.30


Many people will also want access to npm to manage their Node packages. You can also get this from EPEL by typing:

3. sudo yum install npm

https://www.digitalocean.com/community/tutorials/how-to-install-node-js-on-a-centos-7-server
