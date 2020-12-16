color a
cls
@echo off
echo Calculator with .bat 1.0 by YBU

echo Write down the first number you want to calculate:
echo.
set /P number1=
echo.

echo Select the process you want to calculate: ( + - * / )
echo.
set /P action=

if [%action%]==[+] echo Collection process selected
if [%action%]==[-] echo Subtraction process selected
if [%action%]==[*] echo The multiplication operation is selected
if [%action%]==[/] echo Division operation selected

echo.
echo Select the transaction you want to calculate.
echo.
set /P number2=
echo.

set /A result= %number1% %action% %number2
echo.
echo Final Result: %number1% %action% %number2% = '%result%'
pause>nul