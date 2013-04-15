常用命令
--------

Command | Result 
--- | ---
show dbs | 显示数据库列表
db | 显示当前使用的库
use databse | 使用`database`库
db.collection.find() | 检索`collection`
db.collection.remove(`query`, `justOne`) <br> db.collection.remove()| 删除某条记录</br>删除所有记录
show collections | 查询所有表

常用操作
----

Operator | Result
--- | ---
$set | 修改值 db.collection.update( { field: value1 }, { $set: { field1: value2 } } );
$unset | 删除值 db.collection.update( { field: value1 }, { $unset: { field1: "" } } );
$inc | 增值 db.collection.update( { field: value },{ $inc: { field1: amount } } ); <br> `multi`表示所有db.collection.update( { age: 20 }, { $inc: { age: 1 } }, { multi: true } ); <br>db.collection.update( { name: "John" }, { $inc: { age: 2 } }, { multi: true } );
