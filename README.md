# linqQueries
101 linq queries. Credit Microsoft https://code.msdn.microsoft.com/101-LINQ-Samples-3fb9811b

Few additonal revise interview stuff.
https://www.codeproject.com/Articles/744082/WPF-Interview-questions-with-answers

https://www.c-sharpcorner.com/UploadFile/8ef97c/most-asked-wpf-interview-questions-and-answers/

https://docs.microsoft.com/en-us/dotnet/standard/design-guidelines/event

 /* 
 http://www.c-sharpcorner.com/article/most-asked-sql-queries-in-interview-questions/
 
  http://www.sqlservercentral.com/articles/T-SQL/70807/
 
 http://sqlfiddle.com/#!2/22ecb/6
 
 https://livesql.oracle.com/apex/livesql/file/content_O5AEB2HE08PYEPTGCFLZU9YCV.html
 
 https://www.google.co.in/search?q=remove+duplicate+rows+in+sql&oq=remove+duplicate+rows&aqs=chrome.0.0j69i57j0l4.9264j0j4&sourceid=chrome&ie=UTF-8#kpvalbx=1
 
  https://www.codeproject.com/Articles/286255/Using-LINQ-Queries
 
 https://docs.microsoft.com/en-us/dotnet/standard/parallel-programming/task-based-asynchronous-programming
 
 https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/concepts/async/
 
 https://docs.microsoft.com/en-us/dotnet/standard/parallel-programming/task-based-asynchronous-programming
https://www.codeproject.com/Articles/189374/The-Basics-of-Task-Parallelism-via-C
// sample sql fiddle with employee and dept table
http://sqlfiddle.com/#!9/dcb16/1

https://livesql.oracle.com/apex/livesql/file/content_O5AEB2HE08PYEPTGCFLZU9YCV.html
  */
  
  /*
  Azure Design Guide-Must read.
  https://docs.microsoft.com/en-us/azure/architecture/best-practices/auto-scaling


create table dept(  
  deptno     int,  
  dname      varchar(14),  
  loc        varchar(13),  
  constraint pk_dept primary key (deptno)  
);

create table emp(  
  empno    int,  
  ename    varchar(10),  
  job      varchar(9),  
  mgr      int,  
  hiredate datetime,  
  sal      int,  
  comm     int,  
  deptno   int,  
  constraint pk_emp primary key (empno),  
  constraint fk_deptno foreign key (deptno) references dept (deptno)  
);
insert into DEPT (DEPTNO, DNAME, LOC)
values(10, 'ACCOUNTING', 'NEW YORK');

insert into dept  
values(20, 'RESEARCH', 'DALLAS');
insert into dept  
values(30, 'SALES', 'CHICAGO');
insert into dept  
values(40, 'OPERATIONS', 'BOSTON');

insert into emp  
values(  
 7839, 'KING', 'PRESIDENT', null,  
 CONVERT(DATETIME, '1981-11-17'),  
 5000, null, 10  
);

insert into emp  
values(  
 7698, 'BLAKE', 'MANAGER', 7839,  
 CONVERT(DATETIME,'1981-05-01'),  
 2850, null, 30  
);

insert into emp  
values(  
 7782, 'CLARK', 'MANAGER', 7839,  
 CONVERT(DATETIME,'1981-06-09'),  
 2450, null, 10  
);

insert into emp  
values(  
 7566, 'JONES', 'MANAGER', 7839,  
 CONVERT(DATETIME,'1981-4-2'),  
 2975, null, 20  
);

insert into emp  
values(  
 7788, 'SCOTT', 'ANALYST', 7566,  
 CONVERT(DATETIME,'1987-07-13') ,  
 3000, null, 20  
);

insert into emp  
values(  
 7902, 'FORD', 'ANALYST', 7566,  
 CONVERT(DATETIME,'1981-12-3'),  
 3000, null, 20  
);

insert into emp  
values(  
 7369, 'SMITH', 'CLERK', 7902,  
 CONVERT(DATETIME,'1980-12-17'),  
 800, null, 20  
);

insert into emp  
values(  
 7499, 'ALLEN', 'SALESMAN', 7698,  
 CONVERT(DATETIME,'1981-2-20'),  
 1600, 300, 30  
  );
  
  insert into emp  
values(  
 7521, 'WARD', 'SALESMAN', 7698,  
 CONVERT(DATETIME,'1981-2-22'),  
 1250, 500, 30  
);
insert into emp  
values(  
 7654, 'MARTIN', 'SALESMAN', 7698,  
 CONVERT(DATETIME,'1981-9-28'),  
 1250, 1400, 30  
);

insert into emp  
values(  
 7844, 'TURNER', 'SALESMAN', 7698,  
 CONVERT(DATETIME,'1981-9-8'),  
 1500, 0, 30  
);

insert into emp  
values(  
 7876, 'ADAMS', 'CLERK', 7788,  
 CONVERT(DATETIME,'1987-7-13') ,  
 1100, null, 20  
);
insert into emp  
values(  
 7900, 'JAMES', 'CLERK', 7698,  
 CONVERT(DATETIME,'1981-12-3'),  
 950, null, 30  
);
insert into emp  
values(  
 7934, 'MILLER', 'CLERK', 7782,  
 CONVERT(DATETIME,'1982-1-23'),  
 1300, null, 10  
);

    with cte as
    (
      select *,ROW_NUMBER() over (partition by empno order by empno) as RN
      from emp
    ) delete from cte where RN<>1
  */
https://instrumentationtools.com/modbus-communication-interview-questions-answers/

https://instrumentationtools.com/profibus-communication-interview-questions-answers/

https://online.visual-paradigm.com/tutorials/
