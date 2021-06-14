# 03---Data-handling
mysql> INSERT INTO `school` (`name`, `country`, `capacity`) VALUE ('Beauxbatons Academy of Magic', 'France', 550);
mysql> INSERT INTO `school` (`name`, `country`, `capacity`) VALUE ('Castelobruxo', 'Brazil', 380);
mysql> INSERT INTO `school` (`name`, `country`, `capacity`) VALUE ('Durmstrang Institute', 'Norway', 570);
mysql> INSERT INTO `school` (`name`, `country`, `capacity`) VALUE ('Hogwarts School of Witchcraft and Wizardry', 'United Kingdom', 450);
mysql> INSERT INTO `school` (`name`, `country`, `capacity`) VALUE ('Ilvermorny School of Witchcraft and Wizardry', 'USA', 300);
mysql> INSERT INTO `school` (`name`, `country`, `capacity`) VALUE ('Koldovstoretz', 'Russia', 125);
mysql> INSERT INTO `school` (`name`, `country`, `capacity`) VALUE ('Mahoutokoro School of Magic', 'Japan', 800);

mysql> UPDATE school SET country = 'Sweden' WHERE name = 'Durmstrang Institute';
mysql> UPDATE school SET capacity = 700 WHERE name = 'Mahoutokoro School of Magic';

mysql> DELETE FROM school WHERE name LIKE '%Magic%';

mysql> SELECT * FROM school;
+----+----------------------------------------------+----------+----------------+
| id | name                                         | capacity | country        |
+----+----------------------------------------------+----------+----------------+
| 10 | Castelobruxo                                 |      380 | Brazil         |
| 11 | Durmstrang Institute                         |      570 | Sweden         |
| 12 | Hogwarts School of Witchcraft and Wizardry   |      450 | United Kingdom |
| 13 | Ilvermorny School of Witchcraft and Wizardry |      300 | USA            |
| 14 | Koldovstoretz                                |      125 | Russia         |
+----+----------------------------------------------+----------+----------------+
5 rows in set (0,00 sec)
