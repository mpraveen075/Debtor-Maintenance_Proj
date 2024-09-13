# Debtor-Maintenance_Proj
It Is Debtor Maintenance Project By Using Java,Html,Css,JavaScript,JSP,Spring Boot,Hibernate,Spring Data JPA ,Spring Security

change the database name as per your database
change user name and password as per your database

SQL Queries
============

1.User2 Table

CREATE TABLE `user2` (
  `id` int NOT NULL AUTO_INCREMENT,
  `email` varchar(255) DEFAULT NULL,
  `name` varchar(255) DEFAULT NULL,
  `password` varchar(255) DEFAULT NULL,
  `roles` varchar(255) DEFAULT NULL,
  `user_type` varchar(255) DEFAULT NULL,
  PRIMARY KEY (`id`)
) ENGINE=MyISAM DEFAULT CHARSET=utf8mb4 COLLATE=utf8mb4_0900_ai_ci;


2.Debtor_details Table

CREATE TABLE `debtor_details` (
  `debtor_id` int NOT NULL AUTO_INCREMENT,
  `addrline1` varchar(255) DEFAULT NULL,
  `addrline2` varchar(255) DEFAULT NULL,
  `debtor_name` varchar(255) DEFAULT NULL,
  `email` varchar(255) DEFAULT NULL,
  `fax_num` varchar(255) DEFAULT NULL,
  `phone_num` varchar(255) DEFAULT NULL,
  PRIMARY KEY (`debtor_id`)
) ENGINE=MyISAM DEFAULT CHARSET=utf8mb4 COLLATE=utf8mb4_0900_ai_ci;

3. bank_details Table

   CREATE TABLE `bank_details` (
  `debtor_id` int NOT NULL,
  `ifsc` varchar(255) DEFAULT NULL,
  `acc_no` varchar(255) DEFAULT NULL,
  `bank_name` varchar(255) DEFAULT NULL,
  `branch_name` varchar(255) DEFAULT NULL,
  `acc_currency` varchar(255) DEFAULT NULL,
  PRIMARY KEY (`debtor_id`)
) ENGINE=MyISAM DEFAULT CHARSET=utf8mb4 COLLATE=utf8mb4_0900_ai_ci;

4. transaction_details Table

CREATE TABLE `transaction_details` (
  `debtor_id` int NOT NULL,
  `transaction_status` varchar(255) DEFAULT NULL,
  `transaction_date` varchar(255) DEFAULT NULL,
  `transaction_info` varchar(255) DEFAULT NULL,
  `transaction_no` int DEFAULT NULL,
  PRIMARY KEY (`debtor_id`)
) ENGINE=MyISAM DEFAULT CHARSET=utf8mb4 COLLATE=utf8mb4_0900_ai_ci;


   
