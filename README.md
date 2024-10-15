# EMIS-Design

There were numerous facets that were considered in the design of the system

1. Json information (whether within the application bounday or not)
2. Scalability
3. Availability
4. Back up and restore
5. Archiving
6. Deployment
7. Testing
8. Security
9. Caching

The solution has 3 fundamental parts

1. The UI layer which will have containerised dynamic code and static code in a storage such as S3
2. The App layer which will have 2 APIs. One to bring data which is within the application bounday and the other for external (This is assuming that there are these 2 kinds of data. If this will not be the case then one API can be removed)

The design has assumed a simplistic authentication API and not delved into its hosting and scaling.
The design has assumed an API to access internal data. Again there could be another way to access it, such as a GraphQL server in between.
The design has not looked into details of caching and security either. There can be few different ways in this could be achieved.
