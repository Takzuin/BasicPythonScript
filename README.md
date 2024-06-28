Network Ping Tool

This Python script (ping_ips.py) allows you to ping a range of IP addresses within a specified network to check which hosts respond. It uses the os module to execute ping commands and captures the responses.
How to Use

    Input Parameters:
        red: Enter the base IP address of the network (e.g., 192.168.1). If left blank, defaults to 192.168.1.
        rangoInicial: Starting number of the IP address range to ping (e.g., 1).
        rangoFinal: Ending number of the IP address range to ping (e.g., 250).

    Execution:
        The script iterates through each IP address in the specified range (rangoInicial to rangoFinal).
        Uses the ping command (ping -n 1 <ip_address>) to check if an IP address responds.
        If a response is received (rep == 0), the IP address is added to listaIP.
        Prints whether each IP responded ([OK]) or not ([No responde]).

    Output:
        Displays the total number of IPs that responded to ping.
        Lists all IP addresses that responded.

Example

If you run the script with:

    red = "192.168.1"
    rangoInicial = 1
    rangoFinal = 5

It will ping 192.168.1.1 to 192.168.1.5 and output which IPs respond.
Notes

    Ensure your environment supports the os module and the ping command.
    Adjust the network (red), initial (rangoInicial), and final (rangoFinal) values as per your requirements.

Feel free to modify and distribute this script according to your needs.
