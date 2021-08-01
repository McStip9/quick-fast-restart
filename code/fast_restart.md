@echo off

REG QUERY HKU\S-1-5-19\Environment >NUL 2>&1
IF %ERRORLEVEL% EQU 0 goto :START

echo =============================================================================================================
echo This script needs to be executed as an administrator. Right-click the file and select "Run as administrator".
echo =============================================================================================================
echo.
pause >nul
goto :EOF

:START
echo Press any key to start fast restart...
echo.
pause >null
cls
taskkill /f /im explorer.exe
cls
taskkill /f /im dwm.exe
cls
start explorer.exe
cls
IF EXIST=null DEL /F null
cls
echo Fast restart done. Press any key to exit...
echo.
pause >null
exit

:EOF
exit