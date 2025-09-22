（2）使用 IN 子查询查找所修课程编号为 0002、0005 的学生学号、姓名、性别。

select id,name,sex from student_info where id=(select id from grade where course_id in(‘0002’,’0005));![[Pasted image 20240619163922.png]]