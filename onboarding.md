---
title: "INTERACT Onboarding"
author: "Daniel Fuller"
date: '2018-06-18'
output:
  html_document:
    keep_md: yes
  word_document: default
---



## INTERACT Onboarding

> [Remember that there is no geek gene](http://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1006023)

The purpose of this document is to orient and provide guidance for new trainees and collaborators involved with the INTERACT study. Our aim is to make your integration onto the team straight forward, action oriented, and to help you learn new skills. 

This onboarding document is divided into 4 sections: 
1. Glossary
2. R and RStudio
3. Database Connections in RStudio
4. Github

The goal is to point you to existing tutorials or training that will facilitate your work. It is important to remember that you will need to follow the tutorials in detail to get your head around what you are trying to do. Along with the tutorials we will ask that you do activities specific to INTERACT. We will try our best to acknowledge the great people who have contributed to the tutorials you are completing. 

#### Thanks!

- [Jenny Bryan](https://twitter.com/JennyBryan)
- [Amelia McNamara](https://twitter.com/AmeliaMN)

We hope that once you are done, you can confidently use the INTERACT workflow, do awesome analysis, and publish cool papers. 

## Glossary

- Concatenation 
    - In formal language theory and computer programming, string concatenation is the operation of joining character strings end-to-end. For example, the concatenation of "snow" and "ball" is "snowball". In some but not all formalisations of concatenation theory, also called string theory, string concatenation is a primitive notion. [wikipedia](https://en.wikipedia.org/wiki/Concatenation)
- Database
    - A database is an organized collection of data, stored and accessed electronically. Database designers typically organize the data to model aspects of reality in a way that supports processes requiring information, such as (for example) modelling the availability of rooms in hotels in a way that supports finding a hotel with vacancies. [wikipedia](https://en.wikipedia.org/wiki/Database)
- Git
    - Git is a version control system for tracking changes in computer files and coordinating work on those files among multiple people. It is primarily used for source code management in software development, but it can be used to keep track of changes in any set of files. As a distributed revision control system, it is aimed at speed, data integrity, and support for distributed, non-linear workflows. [wikipedia](https://en.wikipedia.org/wiki/Git) 
- Github
    - GitHub Inc. is a web-based hosting service for version control using Git. It is mostly used for computer code.It offers all of the distributed version control and source code management (SCM) functionality of Git as well as adding its own features. It provides access control and several collaboration features such as bug tracking, feature requests, task management, and wikis for every project. [wikipedia](https://en.wikipedia.org/wiki/GitHub) 
- Integrated Development Environment (IDE)
    - An integrated development environment (IDE) is a software application that provides comprehensive facilities to computer programmers for software development. An IDE normally consists of a source code editor, build automation tools, and a debugger. Most modern IDEs have intelligent code completion. You will learning R with the RStudio IDE.  [wikipedia](https://en.wikipedia.org/wiki/Integrated_development_environment)
- Memory
     - In computing, memory refers to the computer hardware integrated circuits that store information for immediate use in a computer; it is synonymous with the term “primary storage”. Computer memory operates at a high speed, for example random-access memory (RAM), as a distinction from storage that provides slow-to-access information but offers higher capacities. If needed, contents of the computer memory can be transferred to secondary storage, through a memory management technique called “virtual memory”.[wikipedia](https://en.wikipedia.org/wiki/Computer_memory)  
- Package  
    - A package is a suitable way to organize your work and, if you want, share it with others. Typically, a package will include code (not only R code!), documentation for the package and for the functions inside, some tests to check everything works as it should, and data sets. The basic information about a package is provided in the DESCRIPTION file, where you can find out what the package does, who the author is, what version the documentation belongs to, the date, the type of license its use, and the package dependencies. [datacamp](datacamp.com/community/tutorials/r-packages-guide#what)   
- Programming Language  
    - A programming language is a vocabulary and set of grammatical rules for instructing a computer or computing device to perform specific tasks. The term programming language usually refers to high-level languages, such as BASIC, C, C++, COBOL, Java, FORTRAN, Ada, and Pascal. Each programming language has a unique set of keywords (words that it understands) and a special syntax for organizing program instructions.  [webopedia](https://www.webopedia.com/TERM/P/programming_language.html)  
- R  
    - R is a programming language and free software environment for statistical computing and graphics that is supported by the R Foundation for Statistical Computing. The R language is widely used among statisticians and data miners for developing statistical software and data analysis. [wikipedia](https://en.wikipedia.org/wiki/R_(programming_language))  
- R package   
    - R packages are collections of functions and data sets developed by the community. They increase the power of R by improving existing base R functionalities, or by adding new ones. For example, if you are usually working with data frames, probably you will have heard about dplyr or data.table, two of the most popular R packages. [datacamp](datacamp.com/community/tutorials/r-packages-guide#what)  
- Server   
    - In computing, a server is a computer program or a device that provides functionality for other programs or devices, called “clients”. This architecture is called the client-server model, and a single overall computation is distributed across multiple processes or devices. Servers can provide various functionalities, often called “services”, such as sharing data or resources among multiple clients, or performing computation for a client. A single server can serve multiple clients, and a single client can use multiple servers. A client process may run on the same device or may connect over a network to a server on a different device. Typical servers are database servers, file servers, mail servers, print servers, web servers, game servers, and application servers.   [wikipedia](https://en.wikipedia.org/wiki/Server_(computing))   
- SQL  
    - SQL is a domain-specific language used in programming and designed for managing data held in a relational database management system (RDBMS), or for stream processing in a relational data stream management system (RDSMS). It is particularly useful in handling structured data where there are relations between different entities/variables of the data. SQL offers two main advantages over older read/write APIs like ISAM or VSAM: first, it introduced the concept of accessing many records with one single command; and second, it eliminates the need to specify how to reach a record, e.g. with or without an index.[wikipedia](https://en.wikipedia.org/wiki/SQL)  
- Syntax  
    - In computer science, the syntax of a computer language is the set of rules that defines the combinations of symbols that are considered to be a correctly structured document or fragment in that language. This applies both to programming languages, where the document represents source code, and markup languages, where the document represents data. The syntax of a language defines its surface form. Text-based computer languages are based on sequences of characters, while visual programming languages are based on the spatial layout and connections between symbols (which may be textual or graphical). Documents that are syntactically invalid are said to have a syntax error.[wikipedia](https://en.wikipedia.org/wiki/Syntax_(programming_languages))  
- Tidy Data  
     - Tidy data is the data obtained as a result of a process called data tidying. It is one of the important cleaning processes during big data processing and is a recognized step in the practice of data science. Tidy data sets have structure and working with them is easy; they’re easy to manipulate, model and visualize. Tidy data sets main concept is to arrange data in a way that each variable is a column and each observation (or case) is a row. Tidy data provides standards and concepts for data cleaning, and with tidy data there’s no need to start from scratch and reinvent new methods for data cleaning.[wikipedia](https://en.wikipedia.org/wiki/Tidy_data)  

## R + RStudio

### Tutorial

https://github.com/AmeliaMN/IntroToR/blob/master/README.md

https://ismayc.github.io/rbasics-book/6-errors.html

https://www.datacamp.com/courses/free-introduction-to-r

### INTERACT Tasks

## R Markdown

### Tutorial
https://www.youtube.com/watch?v=-apyD5f9nwg

https://www.rstudio.com/wp-content/uploads/2015/02/rmarkdown-cheatsheet.pdf

### INTERACT Tasks

## Database Connections in RStudio

### Tutorial

https://support.rstudio.com/hc/en-us/articles/214510788-Setting-up-R-to-connect-to-SQL-Server-

https://db.rstudio.com/rstudio/connections/

### INTERACT Tasks

These are the steps you will need to follow
1. Install PostgreSQL on your system. You can find the necessary files here (https://www.postgresql.org/download/)
2. Install 

You will now setup the connection to the server with the data. You will need to have USask credentials and VPN access to USask. If you have USask credentials you can find information on using the VPN here (https://www.usask.ca/ict/services/network-services/vpn/mac-106-intel-vpn.php). 

**Make sure you are connected to the USask VPN**



You will need to install the following libraries:
```
library(dbplyr)
library(odbc)
library(DBI)
library(RPostgreSQL) 
```    
Now create a connection to the server using the `dbConnect` function. Using the ` rstudioapi::askForPassword("Database user")` and `rstudioapi::askForPassword("Database password")` function allows you to share code without sharing the password. **Never store your password in code!**

```
con <- dbConnect(odbc(),
                 Driver = "SQLServer",
                 Server = "mysqlhost",
                 Database = "mydbname",
                 UID = rstudioapi::askForPassword("Database user"),
                 PWD = rstudioapi::askForPassword("Database password")
                 Port = 1433)
```

We have provided you with a test username and test password for this tutorial. This will allow you to test the connect and make sure you can access the data. There is official INTERACT data here. 

##  RStudio + Github

### Tutorial

http://happygitwithr.com/

### INTERACT Tasks

