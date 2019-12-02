1. Download `mongodb-linux-x86_64-rhel70-v4.2-latest.tgz` from [MongoDB downloading page](https://www.mongodb.org/dl/linux/).
2. Install it to Fedora 30.

Then run following commands.

On one terminal:

```
$ mkdir -p tmp/mdb

$ mongod --dbpath tmp/mdb
```

On anotehr terminal:

```
$ which ruby
/usr/local/ruby-2.7.0-preview3/bin/ruby

$ ruby -v
ruby 2.7.0preview3 (2019-11-23 master b563439274) [x86_64-linux]

$ which bundle
/usr/local/ruby-2.7.0-preview3/bin/bundle

$ bundle -v
Bundler version 2.1.0.pre.3

$ bundle install --path vendor/bundle --without release development

$ vi .rspec
=> Replace "--colour" with "--no-colour".

$ bundle exec rake 2>&1 | tee rake.log
```
