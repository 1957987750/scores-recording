# scores-recording
对已存在的考试成绩，显示为普通文本；对没有输入的考试成绩，则用文本框提供输入；实现分数统计等功能。
1、本题使用的数据库主要包含你以下三个表：
（1）保存学生信息的表T_STUDENT(STUNO,STUNAME,STUNEX)。
（2）保存分数信息的表T_SCORE(STUNO,TYPE,COURSENO,SCORE)。
（3）保存课程信息的表T_COURSE(COURSENO,COURSENAME)。
对于已选课的学生，在T_SCORE表中预先保存了他们的选课信息，因此在输入分数的时候，实际上是对现有记录进行修改。
本题只需要用到一个界面——输入分数界面，但在此系统中编写了两个JSP负责输入显示分数显示界面，另一个负责接受用户输入的分数，并将此分数进行保存，工作完毕后再跳转回第一个JSP。
由于学生的数量事先不可预知，所以将这些分数文本框定义为同名表单元素。另外，对于每个学生的分数输入，还应该用隐藏表单保存该成绩对应学生的学号、课程编号、考试类型。

2、目标页面应该获得以下内容
Courseno:保存课程编号。
Score:保存分数，由于可能会输入多个学生的成绩，所以type应该是含有若干个分数的数组。
Type：保存考试类型，由于可能会输入多个学生的成绩，所以type应该是含有若干个类型的数组。
Stuno:保存分数对应的学生学号，由于可能会输入多个学生成绩，所以stuno应该是含有若干学号的数组。

