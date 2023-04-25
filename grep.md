# grep 실습 

1.

(a) exercise 디렉토리 내에 존재하는 모든 디렉토리 목록

```
ls -la
```



(b) ‘at’ 문자열이 들어간 디렉토리 및 파일의 이름을 출력하라.

```
ls -l|grep 'at'
```





[2-10] ex_datafile 내에서 다음 조건들에 알맞은 행을 출력하라.

2. (a) ‘C’로 시작하는 행

```
grep '^C' ex_datafile
```

​	 (b) 결과로 검색된 행의 수

```
(b) grep -c '^C' ex_datafile
```

3. 문자열 ‘^C’를 포함하는 행

```
grep '\^C' ex_datafile
```

4. (a) ‘Project’를 포함하는 단어가 있는 행

```
grep 'Project' ex_datafile
```

​		(b) ‘Project’와 정확하게 일치하는 단어가 있는 행

```
grep ' Project ' ex_datafile
```

5. 9를 하나 이상 포함하는 행

```
egrep '9+' ex_datafile
```

6. 강의명에 ‘Language’ 또는 ‘Manage’를 포함하는 행

```
grep 'Language\|Manage' ex_datafile
```

7. ‘Design’ 다음에 마침표 1개가 나오고, 숫자가 없거나 또는 1개 나오는 행

```
egrep 'Design\.?[0-9]' ex_data
```

8. 대소문자를 무시하고 문자열 ‘tra’를 하나 이상 포함하는 행

```
grep -i 'tra' ex_datafile
```

9. 소문자 t 다음에 소문자 h나 y 또는 마침표가 나오는 행

```
grep 't[hy.]' ex_datafile
```

10. 3학년, 4학년 과목을 제외하고 출력하라. 

