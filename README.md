Platform of Services 004
========================

A simple platform of servicesbased on Ruby On Rails

I) Installation
---------------

* EDI: Atom
```
sudo apt-get install software-properties-common   # To have add-apt-repository
sudo add-apt-repository ppa:webupd8team/atom 
sudo apt-get update 
sudo apt-get install atom
```

* Ruby Version Manager

https://www.howtoforge.com/tutorial/ubuntu-ruby-on-rails/

```
gpg --keyserver hkp://keys.gnupg.net --recv-keys 409B6B1796C275462A1703113804BB82D39DC0E3 \
7D2BAF1CF37B13E2069D6956105BD0E739499BDB
curl -sSL https://get.rvm.io | bash -s stable --ruby
#source /usr/local/rvm/scripts/rvm
source /home/nfoata/.rvm/scripts/rvm
rvm version

#sudo apt install ruby-railties
```

* Ruby
```
rvm get stable --autolibs=enable
usermod -a -G rvm root
rvm list known
rvm install ruby-2.5.1
rvm --default use ruby-2.5.1
ruby -v
```


* Ruby Gem (Ruby Package Manager)
```
gem update --system
gem -v                #2.7.7
```


* Ruby on Rails (RoR)
```
gem install rails -v 5.2.0
rails -v
```

* MySQL
```
sudo apt-get install mysql-server
sudo ufw allow mysql
systemctl start mysql
systemctl enable mysql

sudo -i
mysql
update user set authentication_string=PASSWORD("YOUR-NEW-ROOT-PASSWORD") where User='root';
flush privileges;
```

https://support.rackspace.com/how-to/installing-mysql-server-on-ubuntu/
https://stackoverflow.com/questions/42421585/default-password-of-mysql-in-ubuntu-server-16-04/49778695

* Postgres
```
sudo apt install postgresql postgresql-contrib -y
```
https://wixelhq.com/blog/how-to-install-postgresql-on-ubuntu-remote-access


