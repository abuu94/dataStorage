# dataStorage
Learn  different RDBMS 

### Links
- https://www.postgresql.org/download/windows/
- https://www.w3schools.com/postgresql/index.php
- https://www.w3schools.com/postgresql/postgresql_install.php

There are several ways to connect to the database, we will look at two ways in this tutorial:
  - SQL Shell (psql)
  - pgAdmin 4

```
CREATE TABLE students (
  studentname VARCHAR(255),
  studentemail VARCHAR(255),
  studentage INT,
  studentaddress VARCHAR(255)
);

CREATE TABLE students (
  studentid INT GENERATED ALWAYS AS IDENTITY PRIMARY KEY,
  studentname VARCHAR(255),
  studentemail VARCHAR(255),
  studentage INT,
  studentaddress VARCHAR(255)
);

CREATE TABLE students (
  studentid SERIAL PRIMARY KEY,
  studentname VARCHAR(255),
  studentemail VARCHAR(255),
  studentage INT,
  studentaddress VARCHAR(255)
);

```

```
INSERT INTO students (studentname, studentemail, studentage, studentaddress) VALUES
('Ali Juma', 'ali.juma@example.com', 20, 'Stone Town'),
('Fatma Said', 'fatma.said@example.com', 22, 'Mbweni'),
('Hassan Omar', 'hassan.omar@example.com', 19, 'Mombasa'),
('Zainab Yusuf', 'zainab.yusuf@example.com', 21, 'Darajani'),
('Salma Khalid', 'salma.khalid@example.com', 23, 'Kijichi'),
('Mohamed Issa', 'mohamed.issa@example.com', 20, 'Makunduchi'),
('Asha Ramadhani', 'asha.ramadhani@example.com', 18, 'Kiembe Samaki'),
('Juma Bakari', 'juma.bakari@example.com', 24, 'Fumba'),
('Rehema Musa', 'rehema.musa@example.com', 22, 'Chukwani'),
('Tariq Abdalla', 'tariq.abdalla@example.com', 21, 'Mtoni'),
('Nadia Suleiman', 'nadia.suleiman@example.com', 20, 'Bububu'),
('Yusuf Ali', 'yusuf.ali@example.com', 19, 'Kisauni'),
('Leila Ahmed', 'leila.ahmed@example.com', 23, 'Kikunguni'),
('Omar Salim', 'omar.salim@example.com', 22, 'Nungwi'),
('Amina Rashid', 'amina.rashid@example.com', 20, 'Paje'),
('Khalid Noor', 'khalid.noor@example.com', 21, 'Jangwani'),
('Saida Mzee', 'saida.mzee@example.com', 19, 'Kizimkazi'),
('Bakari Hassan', 'bakari.hassan@example.com', 24, 'Mwera'),
('Zubeda Ali', 'zubeda.ali@example.com', 22, 'Makadara'),
('Hamza Abdallah', 'hamza.abdallah@example.com', 20, 'Magomeni');
```
