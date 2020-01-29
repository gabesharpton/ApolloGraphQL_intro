# ApolloGraphQL_intro

First install dependencies
Import schema and set up
Connect a REST api

``` npm install apollo-datasource-rest --save ```

Connect Database
Build custom datasource

Here are some of the core concepts for creating your own data source:

- The initialize method: You'll need to implement this method if you want to pass in any configuration options to your class. Here, we're using this method to access our graph API's context.
- this.context: A graph API's context is an object that's shared among every resolver in a GraphQL request. We're going to explain this in more detail in the next section. Right now, all you need to know is that the context is useful for storing user information.
- Caching: While the REST data source comes with its own built in cache, the generic data source does not. You can use our cache primitives to build your own, however!