## Install Node from the EPEL Repository
An alternative installation method uses the EPEL (Extra Packages for Enterprise Linux) repository that is available for CentOS and related distributions.
To gain access to the EPEL repo, you must modify the repo-list of your installation. Fortunately, we can reconfigure access to this repository by installing a package available in our current repos called epel-release.

1. sudo yum install epel-release

2.
For Latest Release:-
yum install -y gcc-c++ make
curl -sL https://rpm.nodesource.com/setup_13.x | sudo -E bash -

For Stable Release:-
yum install -y gcc-c++ make
curl -sL https://rpm.nodesource.com/setup_12.x | sudo -E bash -

3. yum install nodejs
