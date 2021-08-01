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
echo Press any key to start quick restart...
echo.
pause >null
cls
taskkill /f /im StartMenuExperience.exe
cls
taskkill /f /im YourPhone.exe
cls
taskkill /f /im YourPhoneServer.exe
cls
taskkill /f /im vmcompute.exe
cls
taskkill /f /im TabTip.exe
cls
taskkill /f /im SearchIndexer.exe
cls
taskkill /f /im SearchFilterHost.exe
cls
taskkill /f /im SearchProtocolHost.exe
cls
taskkill /f /im smartscreen.exe
cls
taskkill /f /im OfficeClickToRun.exe
cls
taskkill /f /im chrome.exe
cls
taskkill /f /im explorer.exe
cls
taskkill /f /im dwm.exe
cls
start TabTip.exe
cls
start SearchIndexer.exe
cls
start SearchFilterHost.exe
cls
start SearchProtocolHost.exe
cls
start explorer.exe
cls
IF EXIST=null DEL /F null
cls
echo Quick restart done. Press any key to exit...
echo.
pause >null
exit

:EOF
exit