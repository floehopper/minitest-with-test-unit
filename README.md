# MiniTest with Test::Unit

## Ruby 2.0.0

    $ ruby -v
    ruby 2.0.0p0 (2013-02-24 revision 39474) [x86_64-darwin12.2.0]
    
    $ bundle install
    Fetching git@github.com:floehopper/minitest.git
    remote: Counting objects: 2988, done.
    remote: Compressing objects: 100% (1926/1926), done.
    remote: Total 2988 (delta 1333), reused 2515 (delta 897)
    Receiving objects: 100% (2988/2988), 685.46 KiB | 36 KiB/s, done.
    Resolving deltas: 100% (1333/1333), done.
    Fetching gem metadata from https://rubygems.org/........
    Using minitest (5.0.0) from git@github.com:floehopper/minitest.git (at with-gemspec) 
    Using bundler (1.3.5) 
    Your bundle is complete!
    It was installed into ./.bundle/gems
    
    $ bundle exec ruby foo_test.rb
    Warning: you should require 'minitest/autorun' instead.
    From ~/.rbenv/versions/2.0.0-p0/lib/ruby/2.0.0/test/unit.rb:3:in `require'
         ~/.rbenv/versions/2.0.0-p0/lib/ruby/2.0.0/test/unit.rb:3:in `<top (required)>'
         foo_test.rb:3:in `require'
         foo_test.rb:3:in `<main>'
    MiniTest::Unit::TestCase is now Minitest::Test.
    From ~/.rbenv/versions/2.0.0-p0/lib/ruby/2.0.0/test/unit/testcase.rb:8:in `<module:Unit>'
         ~/.rbenv/versions/2.0.0-p0/lib/ruby/2.0.0/test/unit.rb:670:in `<class:Runner>': undefined method `_run_suite' for class `Test::Unit::Runner' (NameError)
    from ~/.rbenv/versions/2.0.0-p0/lib/ruby/2.0.0/test/unit.rb:255:in `<module:Unit>'
    from ~/.rbenv/versions/2.0.0-p0/lib/ruby/2.0.0/test/unit.rb:9:in `<module:Test>'
    from ~/.rbenv/versions/2.0.0-p0/lib/ruby/2.0.0/test/unit.rb:8:in `<top (required)>'
    from foo_test.rb:3:in `require'
    from foo_test.rb:3:in `<main>'

## Ruby 1.9.3

    $ ruby -v
    ruby 1.9.3p362 (2012-12-25 revision 38607) [x86_64-darwin11.4.2]

    $ bundle install
    Fetching git@github.com:floehopper/minitest.git
    remote: Counting objects: 2988, done.
    remote: Compressing objects: 100% (1926/1926), done.
    remote: Total 2988 (delta 1333), reused 2515 (delta 897)
    Receiving objects: 100% (2988/2988), 685.46 KiB | 393 KiB/s, done.
    Resolving deltas: 100% (1333/1333), done.
    Fetching gem metadata from https://rubygems.org/........
    Resolving dependencies...
    Using minitest (5.0.0) from git@github.com:floehopper/minitest.git (at with-gemspec)
    Using bundler (1.3.0)
    Your bundle is complete!
    It was installed into ./.bundle/gems

    $ bundle exec ruby foo_test.rb
    Warning: you should require 'minitest/autorun' instead.
    From ~/.rbenv/versions/1.9.3-p362/lib/ruby/1.9.1/test/unit.rb:3:in `require'
         ~/.rbenv/versions/1.9.3-p362/lib/ruby/1.9.1/test/unit.rb:3:in `<top (required)>'
         foo_test.rb:3:in `require'
         foo_test.rb:3:in `<main>'
    MiniTest::Unit::TestCase is now Minitest::Test.
    From ~/.rbenv/versions/1.9.3-p362/lib/ruby/1.9.1/test/unit/testcase.rb:8:in `<module:Unit>'
         ~/.rbenv/versions/1.9.3-p362/lib/ruby/1.9.1/test/unit.rb:328:in `autorun': uninitialized class variable @@installed_at_exit in Test::Unit::Runner (NameError)
    from ~/.rbenv/versions/1.9.3-p362/lib/ruby/1.9.1/test/unit.rb:640:in `<top (required)>'
    from foo_test.rb:3:in `require'
    from foo_test.rb:3:in `<main>'

