Spring Social Gowalla
=====================
Spring Social Gowalla is an extension to Spring Social for connecting applications
with the Gowalla location-based service.

# IMPORTANT: Project Status
On December 2, 2011, Facebook and Gowalla announced that Facebook
was acquiring Gowalla. The specifics of the acquisition involve Facebook acquiring
several members of the Gowalla team, including Gowalla's founders. Facebook will not,
however, be acquiring Gowalla's technology or data. The Gowalla service will wind
down at the end of January 2012.

With no service to connect to, it makes very little sense to grow or maintain
Spring Social Gowalla any further. While the code will remain in GitHub for
historical purposes, this project had effectively ended and no further work
will be performed here.

Although Spring Social Gowalla will no longer be maintained, Spring Social will
continue to enable applications to connect with Software-as-a-Service sites such
as Facebook and Twitter. If location-based service integration is something you're
interested in, we encourage you to have a look at 
[Spring Social Foursquare](https://github.com/mattupstate/spring-social-foursquare),
a complete Spring Social extension for connecting with Foursquare.

# Getting Spring Social Gowalla
To check out the project and build from source, do the following:

 git clone --recursive git://github.com/SpringSource/spring-social-gowalla.git
 cd spring-social-gowalla
 ./gradlew build

Note: the --recursive switch above is important, as spring-social-gowalla uses
git submodules, which must themselves be cloned and initialized. If --recursive
is omitted, doing so becomes a multi-step process of: 

git clone git://github.com/SpringSource/spring-social-gowalla.git
git submodule init
git submodule update

## Importing into Eclipse
To generate Eclipse metadata (.classpath and .project files), do the following:

 ./gradlew eclipse

Once complete, you may then import the projects into Eclipse as usual:

 File -> Import -> Existing projects into workspace

## Importing into IDEA
To generate IDEA metadata (.iml and .ipr files), do the following:

 ./gradlew idea

## Building the JavaDoc
To build the JavaDoc, do the following from within the root directory:

 ./gradlew :docs:api

The result will be available in 'docs/build/api'.
