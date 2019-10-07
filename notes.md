# to run server
- sudo mongod
- sudo npm run server

# lesson 1
- server.js all code
- Mutations and Queries are like your routes, what your API can do and what ppl can actually use 
- test how they look in the playground

# lesson 2
- all code done in product.gql
- we are doing this to make the tests pass
- enum are hard coded values that cannot change
- npm run test-schema in terminal
- all the tests will fail at first, look what theyre looking for and add the code
- you will find all info needed for the code you are writing in the tests folder, in the product.type.spec file

# Resolvers
- resolvers: resolve queries, mutations, anything of value, enums, etc
- they are like controllers that talk to the db but they resolve all the way down, so if a type referes to a field with another type that refers to another type
- create a resolver in server.js based on the const rootschema you provide
- now run the server and type this into the plaground:
- { cat(name: 'Timmy') { name age owner{ name}, }}