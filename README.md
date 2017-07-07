# CapTech Challenge Three (Swift / iOS)
CapTech code challenge number 3 (Swift / iOS)

#### 1. Assignment
_This assignment, the third in the series, will familiarize the student with storing large amounts of data locally in the app and using the embedded SQL engine. This assignment can be done for iOS, Android, mobile web, or any combination thereof._

#### The application must do the following:
* Store a database of all of the zip codes in the United States along with geographic and demographic information. See the Recommended Approach section for the raw data file.
* The zip code data has a many-to-many relationship between zip code and locality name. One locality may have multiple zip codes and one zip code may have multiple localities.
* The zip code data originates in a CSV file. The application should read and convert this CSV file into a local database only on the first run of the application on the phone. Subsequent runs must use the local database created in the first run. You may pre-convert the data into the appropriate SQL database prior to deployment.
* The user must be able to search by zip code or locality name to find all localities that match.
* Free text queries are not required.
* Users must be able to search by partial zip code or partial locality. Localities are just the city name. _For example, if a user searches for Richmond they should find both Richmond, VA and Richmond, IN._
* The search results must be displayed in a view that displays all of the results without requiring user driven pagination (i.e. infinite tables).
* The view for each entry must display the zip code, city, state, zip
* If the user selects an entry the app must open a new view with a map centered on the locality.
* The map must display a pin centered on the lat/lng of the location.
* If the user taps the map pin the app should transition to a new page that displays the full demographic data for the locality.
* The application must use the embedded SQL engine provided by the platform.
* The application must conform to the HiG of the running device.

#### 2. Assignment Prerequisites
_[Assignment #1](https://github.com/coreyd303/CapTechChallengeOne) and [Assignment #2](https://github.com/coreyd303/CapTechChallengeTwo) of the mobile development boot camp should be completed before starting this assignment._

#### 3. Assignment Objectives
_When completed the student should have an understanding of the following concepts:_

* Embedded SQL engine
* Embedded ORM layer for iOS and Content Providers for Android
* Managing large amounts of data in a small amount of space
* Map Views
* String manipulation

#### 4. Recommended Approach
* Data File: https://portal.captechventures.com/SO/Mobile/TechChallenges/Assignments/free-zipcode-database.csv.zip
_[Local copy of data file]()
* Suggested ERD:

![suggested ERD architecture](erd.png width="100" height="500")

* Web resources:
  * Apple core data docs: https://goo.gl/WC8gOw
  * [Core Data Tutorial](http://www.raywenderlich.com/934/core-data-tutorial-getting-started)
* Required Tools: 
  * XCode 6+
  * Mac with OS X 10.10
* Suggested APIs
  * UITableView
  * UIMapView
  * NSFileManager

#### 3. Getting started

1. Open xcode and start a new project as a single page application
2. Initialize git from the project directory with _git init_
3. Create a gitHub repo for this project
  * Add your project to your new repo

#### 4. Extension Challenges
* TBD