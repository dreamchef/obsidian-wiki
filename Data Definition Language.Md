#databases #software-development

  

defines and modifies structures in a database


# Operations
- `create database <database>` 

- `alter` 

- `drop table <table name>` 
# Examples
```
create table if not exsits <table name> (
	<colname> datatype modifiers,
	<colname> datatype modifiers
);
```
```
alter table < table name>
add column <column name> <data type>;
```
```
alter table < table name>
add constraint <constraint name> < constraint> (<columns>);
```

