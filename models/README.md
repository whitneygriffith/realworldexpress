The models folder will be used for storing our data models. These models will contain the schema for our data and will be the entry point for how our data gets in and out of our database.

# Data Management

- Define and Register our data schema
- Ensures [data validations](https://mongoosejs.com/docs/validation.html) 
- Ensures data remains consistent throughout application
- Timestamps data changes 
 
# Database 

## No SQL 

[Mongo DB](https://www.mongodb.com/) and its object modeler [Mongoose](http://mongoosejs.com)

[Cosmos DB](https://docs.microsoft.com/en-us/azure/cosmos-db/sql-api-nodejs-application) and its object modeler [Cosmos DB Client Library](https://www.npmjs.com/package/@azure/cosmos)

[Firebase Data Store](https://firebase.google.com/docs/firestore) and its numerous object modelers:
- [fireorm](https://www.npmjs.com/package/fireorm)
- [typesaurus](https://www.npmjs.com/package/typesaurus)
- [firebase-firestorm](https://www.npmjs.com/package/firebase-firestorm)
- [ORMOnFire](https://www.npmjs.com/package/@typeheim/orm-on-fire)

## Models Development

*Using User as an example of a new Model*

* Create a new file `User.js`

* Create the schema for the *User Model* in `User.js`

* Add validations to the *User Model* such as:
    * Email REGEX
    * Unique validation

* Create helper methods on the *User Model* such as: 
    
    * Set and validate passwords 
    * Generate JWTs. JWT's are the tokens that will be passed to the front-end that will be used for authentication. The JWT contains a payload (assertions) that is signed by the back-end, so the payload can be read by both the front-end and back-end, but can only be validated by the back-end.

* Register *User Model* with application, `app.js`





