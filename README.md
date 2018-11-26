# mysql_bot_core_seen_system
Seen System for MySQL Bot Core

This is a module for MySQL Bot Core system.
You'll need https://github.com/thistehneisen/mysql_bot_core in order for this to work.

[12:02] <Neisen> !seen wubwubwub
[12:02] -#DEV-SQL- Last seen wubwubwub before 34secs changing nickname to Hawkee

MySQL Database Structure:

```
CREATE TABLE `seen` (
  `nickname` varchar(50) NOT NULL,
  `address` varchar(200) NOT NULL,
  `time` datetime NOT NULL,
  `network` varchar(50) NOT NULL,
  `action` enum('j','p','q','n','a','t') NOT NULL,
  `extra` varchar(100) NOT NULL,
  PRIMARY KEY (`nickname`)
) ENGINE=InnoDB DEFAULT CHARSET=latin1;
```
