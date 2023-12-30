# **新增CODE 及工单填写sql样例**

系统中新增code 通常会涉及到这三个表 
但是在工单中的插入数据时需要select 查出数据并插入数据
```sql
select * from fw.CODE_CONFIG;
select * from fw.CODE_DOC;
select * from fw.CODE_LIST;


insert into fw.code_config (DBID, DMBH, CODE, CONTENT, XH)
select dbid, 'ZWZT', '2', '已取消', null
from fw.dbid_info;

insert into fw.code_doc (DMBH, CODE, CONTENT, SM)
values ('ZWZT', '2', '已取消', '');

insert into fw.code_list (DMBH, DMMC, DMSM, DMSYFW)
values ('XXSHSX', '信息审核顺序', '资格审核和照片审核的先后顺序', '10');

```


