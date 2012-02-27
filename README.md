# Rails on Heroku with JRuby

Warning: This is not for production use. 

Tested with:

* Rails 3.2.1
* JRuby 1.6.7 (1.9 mode)
* trinidad 

## Benchmark

http://i.imgur.com/Hk9X9.png

The result is probably worse than one thin/unicorn on one dyno. And one dyno can run 3-4 unicorns.

## Known issues

* Error H99 (Platform error) encountered.
* Memory warnings were received for larger applications because of the 512MB memory limit on heroku.

## Based on 

* http://chris.chowie.net/2011/08/28/Sinatra-with-JRuby-on-Heroku/
* https://github.com/Soliah/sinatra-jruby-heroku
