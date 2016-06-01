# MiniMongoLibre
Cloned from [eface2face's](https://github.com/eface2face/meteor-minimongo) NPM wrapper of Meteor's [MiniMongo](https://www.meteor.com/mini-databases), to create a version which is completely decoupled from the Meteor MiniMongo.

This project is still under development, so is yet to be published on NPM. For now you will need to clone the project, run `npm install` and use browserify.

Create a collection using the following steps

    var minimongo = require("./node_modules/minimongolibre")();
    var collectionName = new minimongo.LocalCollection("collectionName");
Once you have done this, simply follow the [MiniMongo API](http://guide.meteor.com/collections.html) - findOne, find, insert etc.

This database system is volatile meaning all data will be lost when you close the browser. The next step in this project will be to examine the best way to allow you to reactively communicate the state of the database, as is done in Meteor. 