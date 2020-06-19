## **Data Modeling with Apache Cassandra**
-----------------------------------------------------------------------------------------------------------------------------------

In this project, I will build an ETL pipeline using Python with the focus on Apache Cassandra and how it is different from relational database data modeling.

Cassandra primary keys is made up of Partion Keys or Clustering Columns.Data with the same Primary Key will be overwritten. In Where conditions the Primary Key must be included and you can use Clustering Columns to order your data.

In Cassandra the denormalization process is a must, you cannot apply normalization like an RDBMS 
because you cannot use JOINs. More the denormalization process is done more the query will 
run faster, in fact, Cassandra has been optimized for fast writes not for fast reads. 

I will process the event_datafile_new.csv dataset to create a denormalized dataset


Using provided queries, I will model the data tables

Load the data into tables created in Apache Cassandra and run provided queries
## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. The following steps are tested only for Ubuntu 18.04.

### Docker

This project comes with a docker container with Apache Cassandra and the necessary database (sparkifydb). To get the container up and running, please execute:

```
docker-compose up
```
