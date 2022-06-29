---
id: luppcqjfqye3juy4tv7i4ym
title: data definition language (DDL)
desc: ''
updated: 1656449815987
created: 1654530812779
---
#databases #software-development 

defines and modifies structures in a database

# Operations
| statement | description |
|---|---|
| `create database <database>` |
| `alter` | |
| `drop table <table name>` | |
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

