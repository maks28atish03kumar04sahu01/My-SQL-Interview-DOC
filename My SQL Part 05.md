## Like Operator

### like ‘a%’ Value Starts With “a” 

``` sql
select empname from employeedemodb where empname like 'A%';
```

### like ‘%a’ Value Ends With “a” 

``` sql
select empname from employeedemodb where empname like '%A';
```

### like ‘%am%’ Value having “am” in any position 

``` sql
select empname from employeedemodb where empname like '%ar%';
```

### like ‘a%m’ Value Starts With “a” and end with “m” 

``` sql
select empname from employeedemodb where empname like 'a%r';
```

### like ‘_a%’ “a” in second position of value 

``` sql
select empname from employeedemodb where empname like '_a%';
```

### like ‘__a%’ “a” in third position of value 

``` sql
select empname from employeedemodb where empname like '__a%';
```

### like ‘_am%’ “a” in second position and “m” in third position of value 

``` sql
select empname from employeedemodb where empname like '_ar%';
```

## Regular Expression

### ^  -> ‘^ra’ Value starts with ‘ra’ 

``` sql
select empname from employeedemodb where empname regexp '^am';
```

### $ -> ‘an$’ Value ends with ‘an’ 

``` sql
select empname from employeedemodb where empname regexp 'ar$';
```

### […] -> ‘[rms]’ Values which have ‘r’ or ‘m’ or ‘s’ in any position 

``` sql
select empname from employeedemodb where empname regexp '[vx]';
```

### ^[…] -> ‘^[rms]’ Values which have ‘r’ or ‘m’ or ‘s’ in starting position 

``` sql
select empname from employeedemodb where empname regexp '^[uvx]';
```

### […]$ -> ‘[rat]$’ Values which have ‘r’ or ‘a’ or ‘t’ in ending position 

``` sql
select empname from employeedemodb where empname regexp '[ahi]$';
```

### [a-z] -> ‘[a-h]e’ Values from ‘a’ to ‘h’ which have ‘e’ in any position 

``` sql
select empname from employeedemodb where empname regexp '[a-h]e';
```

### P1 | P2 | P3	Tom | Doc | Hari	Value matches of the pattern ‘Tom’ or ‘Doc’ or ‘Hari’ 

``` sql
select empname from employeedemodb where empname regexp "Neha";
```

``` sql
select empname from employeedemodb where empname regexp "ha | sh";
```






