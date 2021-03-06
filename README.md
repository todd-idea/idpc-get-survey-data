# IDEA Data Portal Command Line Client - Get Survey Data
The idpc-get-survey-data application provides a command line client for
retrieval of report data from the IDEA Data Portal. To use this, you must have
an IDEA Data Portal account (application and key). In addition, this
application assumes that there is survey data already available.

## Project Dependencies
This project is implemented with Groovy and uses Gradle as the build tool.
Therefore, you need to be sure to install the following:
* [Git](http://git-scm.com/downloads)
* [Java (version 6+)](http://www.oracle.com/technetwork/java/javase/downloads/index.html)
* [Groovy](http://groovy-lang.org/)
* [Gradle](http://gradle.org/installation) (or use [GVM](http://gvmtool.net/) to install Gradle)

## Getting Started
* Setup the project
  * Checkout the project: *git clone git@github.com:todd-idea/idpc-get-survey-data.git*
* Run the application
  * Running the application requires a registered IDEA Data Portal application. You must provide the application name and key.
    * -a 'AppName'
    * -k 'AppKey'
  * Running the application requires survey data. You must provide the survey ID.
    * -sid surveyID
  * The application has some optional command line arguments that configure the behavior
    * -h 'host.name' - defines the host where the IDEA Data Portal is (defaults to localhost)
    * -p port - defines the port that the IDEA Data Portal is listening on (default to 8091)
    * -st - configures the collection, and printing, of timing information
    * -v - configures verbose output
    * -s - configures the use of SSL
    * -t - configures the type of report to query (default to ALL)