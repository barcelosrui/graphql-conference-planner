
#Before you get started
- npm i or yarn 
- ng serve => app will be running on port 4200
- To read the schema documentation hosted on graph.cool
- go into the /schema directory and run 
- npm install && npm start 
- or
- yarn && yarn start

//TODO
- You first have to create the apolloClient in apollo.config.ts
- And use this client in the app.module.ts


### 1. Basic queries: Get all conferences 
- What you will learn:
  - Write a query
- Todo:
  - Write a query to fetch all conference using glq tags in 
    conference.apollo-query.ts. You will find all fields required in the 
    conference-card.component.html
  - Use the query in conference-card-list.component.ts

### 2. Basic queries: Conference details
- What you will learn:
  - Understand how you can add variables to your queries/mutations 
  - Understand how variables are used in the query function and in the query itself
  (the id should be required)
- TODO:
  - Write a query to fetch the details of a conference (DetailedConferenceQuery
    in conference.apollo-query.ts . You will find all fields required in the 
    conference-details-level.component.html and sponsor-box.component.html
  - In ConferenceDetails: Implement all todos :p
    Hint: to create the speaker array, you should look at the talks fields

### 3. Basic mutations : Authentication ( Register/ login button)
- What you will learn:
  - Write a basic mutation
  - Understand how variables are passed in mutations
  - Understand how the mutation is available in your component
- TODO:
  - Fix the register and login components by implementing all todos
 
### 4. Advanced queries PART 1
- What you will learn:
  - Mixin mutations and queries in one component
  - Write a query to get the list of conferences on a particular page
  - Write a mutation to delete a conference
  - Understand how you pass variables
  - Understand how apollo passes data in component
  - Understand pagination
- TODO (Don't take care of the Conference component, YET!)
  - In the conference-table-list component, fix all todos
  - In the talks-table-list component, fix all todos

### 5. Advanced queries PART 2
  - The management/Conference component should add a conference if there's no
  conference id in the path params.
  - If there's an id in the path, it means you need to fetch that conference
  and when submitting, you don't need to add it, but update it.
  - Understand skip property
  - Understand name property
  - Mixin mutations and queries

  - Same for management/Talk component

#### Try to decouple your queries by using fragments


## Backend

- Want to see how a schema is written in nodeJS?
- Add another apolloClient to your application with the schema you will create.
- This graphQL editor enables you to create your schema and use it in your app :
- https://launchpad.graphql.com/

- The uri of your schema will be visible in the black bottom part, once you save your project.

- The only thing you have to write now, it a chat application in each conference detail.
Good luck

