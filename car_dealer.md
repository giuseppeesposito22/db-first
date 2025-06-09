| name                 | type                                                   | attributes                         | index       |
| -------------------- | ------------------------------------------------------ | ---------------------------------- | ----------- |
| id                   | BIGINT                                                 | NOT NULL, AUTO_INCREMENT, UNSIGNED | PRIMARY KEY |
| brand                | VARCHAR(50)                                            | NOT NULL                           |             |
| model                | VARCHAR(50)                                            | NOT NULL                           |             |
| year_of_registration | YEAR                                                   | NOT NULL                           |             |
| kilometres           | INT                                                    | NOT NULL, UNSIGNED                 |             |
| fuel_type            | ENUM (Benzina, Diesel, Ibrida, Elettrica, GPL, Metano) | NOT NULL                           |             |
| transmission         | ENUM (Manuale, Automatico)                             | NOT NULL                           |             |
| price                | DECIMAL(6,2)                                           | NOT NULL                           |             |
| color                | VARCHAR(30)                                            | NULL                               |             |
| plate                | CHAR(7)                                                | NOT NULL, UNIQUE                   | INDEX       |
| chassis_number       | CHAR(17)                                               | NOT NULL, UNIQUE                   | INDEX       |
| available            | BOOLEAN                                                | DEFAULT (true)                     |             |
