# Port Scanner

This is the boilerplate for the Port Scanner project. Instructions for building your project can be found at https://www.freecodecamp.org/learn/information-security/information-security-projects/port-scanner

We are still developing the interactive instructional part of the Python curriculum. For now, here are some videos on the freeCodeCamp.org YouTube channel that will teach you everything you need to know to complete this project:

[Python for Everybody Video Course](https://www.freecodecamp.org/news/python-for-everybody/) (14 hours)

[Learn Python Basics in Depth](https://www.freecodecamp.org/news/learn-python-basics-in-depth-video-course/) (4 hours)

[Intermediate Python Course](https://www.freecodecamp.org/news/intermediate-python-course/) (6 hours)

Create a port scanner using Python.

In the port_scanner.py file, create a function called get_open_ports that takes a target argument and a port_range argument. target can be a URL or IP address. port_range is a list of two numbers indicating the first and last numbers of the range of ports to check.

Here are examples of how the function may be called:

```
get_open_ports("209.216.230.240", [440, 445])
get_open_ports("www.stackoverflow.com", [79, 82])
The function should return a list of open ports in the given range.

```

The get_open_ports function should also take an optional third argument of True to indicate "Verbose" mode. If this is set to true, the function should return a descriptive string instead of a list of ports.

Here is the format of the string that should be returned in verbose mode (text inside {} indicates the information that should appear):

```
Open ports for {URL} ({IP address})
PORT     SERVICE
{port}   {service name}
{port}   {service name}

```

You can use the dictionary in common_ports.py to get the correct service name for each port.

For example, if the function is called like this:

port_scanner.get_open_ports("scanme.nmap.org", [20, 80], True)
It should return the following:

Open ports for scanme.nmap.org (45.33.32.156)
PORT     SERVICE
22       ssh
80       http
Make sure to include proper spacing and new line characters.

If the URL passed into the get_open_ports function is invalid, the function should return the string: "Error: Invalid hostname".

If the IP address passed into the get_open_ports function is invalid, the function should return the string: "Error: Invalid IP address".

## Development
Write your code in port_scanner.py. For development, you can use main.py to test your code.

## Testing
The unit tests for this project are in test_module.py. We imported the tests from test_module.py to main.py for your convenience.

## Submitting
Copy your project's URL and submit it to freeCodeCamp.