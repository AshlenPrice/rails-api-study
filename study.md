# Rails as an API Study

Use your favorite search engine and the provided readings to research and
respond to the following questions.

In your responses, be sure to cite any relevant sources you consulted in your
search. We ask you to write responses in your own words in order to see how you
process what you've read. Please do not respond with direct quotes from source
material. Instead, digest what you've read and repeat it in your own voice.

Please note:

-   Many of the readings will mention the "view" layer. We won't be covering the
    view layer in this program.
-   We'll use our [Rails API Template](https://github.com/ga-wdi-boston/rails-api-template)
    repository as the basis for our rails applications.
    This template excludes the "view" layer.

## Required Readings

-   Better Explained
    -   [Starting Ruby on Rails: What I Wish I Knew](http://betterexplained.com/articles/starting-ruby-on-rails-what-i-wish-i-knew/)
        (sections 3 and 4)
    -   [Intermediate Rails: Understanding Models, Views and Controllers](http://betterexplained.com/articles/intermediate-rails-understanding-models-views-and-controllers/)
        (up to and including "Quick Controllers")
-   Ruby on Rails Guides
    -   [Rails Routing from the Outside](http://guides.rubyonrails.org/routing.html)
        (up to and including chapter 2.6)
    -   [Action Controller Overview](http://guides.rubyonrails.org/action_controller_overview.html)
        (up to and including chapter 4.5)
    -   [The Rails Command Line](http://guides.rubyonrails.org/command_line.html)
        (up to and including chapter 1.4)

## Additional Resources

-   [Getting Started with Rails — Ruby on Rails Guides](http://guides.rubyonrails.org/getting_started.html)

## Define Model Responsiblities

In your own words, define what the responsibilities of the model layer are in
Rails.

``` md
The models are responsible for talking to that database, and store  processes information then it sends the information back up to the controllers.

```

## Define Controller Responsiblities

In your own words, define what the responsibilities of the controller layer are
in Rails.

```md
The controller parses the user's requests and it produces the right output. The controller talks to the model and also produces the response back to the client.

```

## Define Router Responsiblities

In your own words, define what the router does in Rails.

```md
The router's job is to parse HTTP requests from the client and send the right thing back to the right controller.
```

## The Request-Response Cycle in Rails

Starting with a client making a GET request to a particular URL, describe how
the parts of Rails interact to produce and send a response.

```md
1. Client sends GET request to server
2. Server parses the request and sends to the controller.
3. Controller gets the request and sends it to the model.
4. Model gets the request parses it and gets the information it needs from the database.  Then DB sends back a Ruby object.
5. Controller converts the  Ruby object into JSON and returns it to the server.
6. Server takes the JSON and  displays it to the client in the appropriate format.

```
