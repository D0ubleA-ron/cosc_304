# COSC 304 - Introduction to Database Systems<br>Lab 4: Building ER diagrams using an UML modeling tool

This lab designs ER diagrams in UML notation using [astah](http://astah.net/editions). <strong>Note: Astah no longer has a free community version. Request a student license or use the 30-day trial.</strong> <a href="https://diagrams.net/">diagrams.net</a> is an online drawing tool that can also be used but it does not have as good support for database modeling in UML.</p>

## Question #1 (10 marks)

Construct a database design in UML for an app store described below. **Data types are not needed.**

- A `Publisher` where each publisher is identified by an <tt>id</tt> and has a `name`. (1 mark)

- A `Category` where each ingredient has an `id`, a `name`, and may have a parent category. (2 marks)

- An `App` storing each app that is identified by a field called <tt>id</tt> and other attributes include `name` and `description`. An App is created by one Publisher. A Publisher may publish multiple Apps. An App has a Category. (3 marks)

- A `AppVersion` stores each version of the app. An AppVersion is associated with exactly one App. Use a `version` field to identify between versions of the same App. Each AppVersion has a `releaseDate`, a `rating`, a `price`, and a `description` (2 marks)

- A `AppVersionReview` stores ratings for each application version. Each instance applies to a single AppVersion, and different reviews are identified by `reviewer` attribute (which is name of reviewer). There is also a `reviewDate`, `rating`, and `review`. (2 marks)


## Question #2 (10 marks)

Construct a database design in UML for a medical system described below. **Data types are not needed.**

- There are multiple hospitals in the medical system. A hospital is identified by its name and has a location. (1 mark)</li>

- A doctor is identified by his medical number and has a name. Each hospital has a single doctor as a manager, and a doctor may manage only one hospital. Doctors are located in hospitals. A doctor may be located in more than one hospital. A doctor located at a hospital has an office number and a salary paid by that hospital. (3 marks)

- A patient is identified by their health id and also has a name and gender. (1 mark)

- A patient visits a doctor at a particular hospital. Each visit is identifed by its own id and also has a visit date. (3 marks)

- At a visit zero or more tests are run each with a cost and an outcome. Each test is identified for a particular visit by name. (2 marks)
