# Mysql


#Create Store procedure


```DROP PROCEDURE xxxxxx;

DELIMITER //

CREATE PROCEDURE `xxxxxx`(IN `pay_id` INT(11), IN `user_id` INT(11), IN `procedure_name` VARCHAR(100), IN `trans_typesss` INT(11), IN `cr_acc_desc` VARCHAR(3000), IN `dr_acc_desc` VARCHAR(3000), IN `pay_mode` INT(11), IN `aff_id` INT(11), IN `amount` DECIMAL(10,2), IN `in_member_id` INT(11), OUT `msg` TEXT)

COMMENT 'test'

BEGIN

--   
    
END//

DELIMITER ;
```


SET TRANSACTION ISOLATION LEVEL READ UNCOMMITTED


```
SET GLOBAL table_definition_cache = 4000; 

SET GLOBAL sql_mode=(SELECT REPLACE(@@sql_mode,'ONLY_FULL_GROUP_BY',''));
```
