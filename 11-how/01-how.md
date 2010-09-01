!SLIDE
# How

!SLIDE 
# Trust

!SLIDE
# How much do you trust the code?

!SLIDE
# Ask your code a question

!SLIDE
# Check the answer

!SLIDE
# Asking a good question is important

!SLIDE
    @@@ ruby 
    Code.awesome? 
     => true

# Done

!SLIDE center
# Ask a simple question
    @@@ ruby
    [1, 2, 3].size == 3

!SLIDE
# What is too simple?

!SLIDE center
# Ask a complicated question
    @@@ ruby
    @me.uncle.cousin.grandmother.neice
       .roomate.dog.breed == 'shelty'

!SLIDE
# What is too complicated?

!SLIDE
# Ask an appropriate question
    @@@ cucumber
    When I register on the site
    Then there should be 47 users

!SLIDE
# Ask an appropriate question
    @@@ cucumber
    When I register on the site
    Then there should be one more user

!SLIDE
# Ask an appropriate question
    @@@ cucumber
    When I register on the site
    Then I can log in

!SLIDE
# What is a redundant question?
### [http://mocha.rubyforge.org/examples/mocha.html](http://mocha.rubyforge.org/examples/mocha.html)

!SLIDE
    @@@ ruby
    class Enterprise
      def go(warp_factor)
        warp_factor.times {
          @dilithium.nuke(:anti_matter)
        }
      end
    end
    class EnterpriseTest < Test::Unit::TestCase
      def test_should_boldly_go
        dilithium = mock()
        dilithium.expects(:nuke)
                 .with(:anti_matter)
                 .at_least_once
        enterprise = Enterprise.new(dilithium)
        enterprise.go(2)
      end
    end

!SLIDE center
# Why not just ask
    @@@ ruby
    line(5) == "warp_factor.times{ ... }"

!SLIDE center
# Oops ... I opinioned
![Oops](oops.jpg)

