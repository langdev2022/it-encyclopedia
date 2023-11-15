m4 preprocessor 
defining parameter_field_list is easy to create pre-sql 

 UPDATE t_parameter 
    SET update_set2({parameter_field_list},{add_prefix_to_list({parameter_field_list},{:NEW.})})
  WHERE  id_parameter=123;


Expression after processing

UPDATE t_parameter 
SET «ID_CONFIG»=:NEW."ID_CONFIG" 
,"ID_OBJECT"=:NEW."ID_OBJECT" 
,"MONIKER"=:NEW."MONIKER" 
,"NAME"=:NEW."NAME" 
,"VALUE"=:NEW."VALUE" 
,"COMMENTS"=:NEW."COMMENTS" 
,"SYS_LEVEL"=:NEW."SYS_LEVEL" 
,"KIND"=:NEW."KIND"  
WHERE id_parameter=123;

cf sendmail file
