chapter 7: code.org
==============================



    sudo apt-get update
    sudo apt-get install -y git mysql-server mysql-client libmysqlclient-dev libxslt1-dev libssl-dev zlib1g-dev imagemagick libmagickcore-dev libmagickwand-dev openjdk-9-jre-headless libcairo2-dev libjpeg8-dev libpango1.0-dev libgif-dev curl pdftk enscript libsqlite3-dev phantomjs build-essential redis-server rbenv ruby-build npm ruby2.3-dev
        Hit enter and select default options for any configuration popups, leaving mysql passwords blank
    Install Node and Nodejs
        Type curl -sL https://deb.nodesource.com/setup_6.x | sudo -E bash -
        And then sudo apt-get install -y nodejs
    Install Ruby 2.2.3 with rbenv
        rbenv install 2.2.3
        rbenv global 2.2.3
        rbenv rehash
    Install yarn
        First, type curl -sS https://dl.yarnpkg.com/debian/pubkey.gpg | sudo apt-key add -
        Then echo "deb https://dl.yarnpkg.com/debian/ stable main" | sudo tee /etc/apt/sources.list.d/yarn.list
        And lastly, sudo apt-get update && sudo apt-get install yarn=0.23.2-1
    Finally, configure your mysql to allow for a proper installation. You may run into errors if you did not leave mysql passwords blank
        Type echo "ALTER USER 'root'@'localhost' IDENTIFIED WITH mysql_native_password BY '';" | sudo mysql

echo "ALTER USER 'root'@'localhost' IDENTIFIED WITH mysql_native_password BY 'king0733';" | sudo mysql
>mysql -uroot -p

>ALTER USER 'root'@'localhost' IDENTIFIED WITH mysql_native_password BY '';
>FLUSH PRIVILEGES;

    Read the following notes, then go back up to the overview and run the commands there.
        If, for any reason, you are forced to interrupt the rake install command before it completes, cd into dashboard and run bundle exec rake db:drop before trying rake install again
        rake install must always be called from the local project's root directory, or it won't work.
        Finally, don't worry if your versions don't match the versions in the overview if you're following this method; the installation should still work properly regardless


GRANT ALL PRIVILEGES ON *.* TO 'root'@'%' IDENTIFIED BY 'king0733' WITH GRANT OPTION;

FLUSH PRIVILEGES;





1.error
 ruby
mkmf.rb can't find header files for ruby at /usr/lib/ruby/include/ruby.h

===>
sudo apt-get install ruby-dev

 sudo apt-get update
 sudo apt-get build-essential

1.1 zlib is missing; necessary for building libxml2
sudo apt-get install zlib1g-dev

1.2  Can't install RMagick 2.15.4. Can't find Magick-config or pkg-config
sudo apt-get install libmagickwand-dev imagemagick

1.3 Installing sqlite3 1.3.11 with native extensions
Gem::Ext::BuildError: ERROR: Failed to build gem native extension.

apt-get install libsqlite3-dev


start

