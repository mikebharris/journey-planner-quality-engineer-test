# Train Timetable testing problem

## The background
You have been brought in as a quality engineer on an existing project to build an application to help people plan their train journeys on the Great Western Railway line, which runs from London into the South-West of England.

The developers have already written code in Java but claimed that they didn't have time to write the tests!

## Your job

Your job is to work out what we could use to write unit tests in Java for the existing code.  The scenarios for the unit tests are outlined in the __Acceptance Criteria__ section below.

* You may use Google, ChatGPT or any another other resource to find reference resources for Java and unit testing.  
* As these are unit tests we do not foresee the need for using Cucumber/Gherkin for these tests, but that is entirely up to you.  We will be interested in the decision you make and the justification for it.
* The full train timetable for testing is provided in the [TestData](src/test/java/journey_planner/TestData.java) Java class.
* We would expect you to write at least one test per acceptance criterium.
* It should be possible to run the tests using `gradle clean test` (Linux/Mac) or `./gradlew clean test` (Windows)
* We welcome any comments you have about the existing code, and this exercise, should you wish to provide them.
 
## Acceptance Criteria
|Criterion|Given|When|Then|
|---|-----|----|----|
|*Report Duration Of Journey Between Two Stations*|The 0907 train from Camborne is scheduled to reach Exeter St Davids at 1137|I ask for the journey time from Camborne to Exeter St Davids if I am at the station at 0907|I am told it will take 150 minutes|
|*Report Duration For First Available Train*|The 0907, 1023 and 1112 trains from Camborne are scheduled to reach Exeter St Davids at 1137, 1302 and 1357, respectively|I ask for the journey time from Camborne to Exeter St Davids if I am at the station at 1023|I am told it will take 159 minutes|
|*Report Duration Including Waiting Time On Platform*|The 0944, 1100 and 1150 trains from St Austell are scheduled to reach Par at 0951, 1108 and 1157, respectively|I ask for the journey time from St Austell to Par if I am at the station at 1101|I am told it will take 56 minutes|
