Proxy Tester



A powerful Python script for testing proxy connections to multiple hosts, featuring a sleek interface with a blinking circle progress bar and colorful output. Developed by TOpPLUG, this tool is designed for efficiency and ease of use, supporting both single domains and bulk testing via file input.

Features





Multi-threaded Testing: Test multiple hosts concurrently with configurable thread counts.



Colorful Output: Gradient-colored progress bar and status messages for clear visibility.



Animated Progress Bar: Displays a blinking circle (⬤ ◯ ◎) with real-time percentage updates.



Flexible Input: Test comma-separated domains or load hosts from a text file.



Response Logging: Saves results to log files (success_200.log, too_many_requests_429.log, bad_gateway_502.log).



Custom Proxy Support: Configurable proxy host and port for testing.



Interactive Interface: Option to run multiple tests in a loop with a clean, styled UI.

Requirements





Python 3.6+



Required Packages:





colorama: For colored terminal output.



pystyle: For gradient text and banner styling.

Install dependencies using:

pip install colorama pystyle

Installation





Clone the repository:

git clone https://github.com/TOpPLUG/Hubdarkweb.git
cd Hubdarkweb



Install the required Python packages:

pip install -r requirements.txt



Ensure you have a working proxy server (default: 157.240.195.32:8080).

Usage

Run the script with:

python proxy_tester.py





Enter Thread Count: Specify the number of concurrent threads (default: 10).



Provide Hosts: Input domains (e.g., google.com,youtube.com) or a path to a text file (e.g., hosts.txt).



View Results: The script displays a colorful banner, a blinking progress bar, and detailed results for each host.



Log Files: Successful (HTTP 200), rate-limited (429), and bad gateway (502) responses are logged to separate files.



Repeat or Exit: Choose to test again or exit the program.

Example Input

Enter number of threads (default 10):
> 5
Enter domain(s) (comma separated) or path to a file:
Examples: google.com,youtube.com OR hosts.txt
> google.com,youtube.com,example.com

Example Output

[google.com] - HTTP 200
-----------------------------------------------------------------
✓ HTTP 200 response (0.12s)
Response: HTTP/1.1 200 OK...
-----------------------------------------------------------------
Progress: ⬤ 3/3 (100.0%)
-----------------------------------------------------------------
✓ Total successes (HTTP 200): 2
✗ Total failures or others: 1
-----------------------------------------------------------------
Test again? (y/n)
> n
Thank you for using Proxy Tester!
Developed by TOpPLUG
GitHub: https://github.com/TOpPLUG/Hubdarkweb
Discord: https://discord.gg/Hub7s

Configuration





Proxy Settings: Modify PROXY_HOST and PROXY_PORT in proxy_tester.py to use your preferred proxy server.

PROXY_HOST = "157.240.195.32"
PROXY_PORT = 8080



Log Files: Results are saved to:





success_200.log: Hosts with HTTP 200 responses.



too_many_requests_429.log: Hosts with HTTP 429 responses.



bad_gateway_502.log: Hosts with HTTP 502 responses.

Contributing

Contributions are welcome! Please:





Fork the repository.



Create a new branch (git checkout -b feature-name).



Submit a pull request with a clear description of changes.

Report issues or suggest features on the GitHub Issues page.

License

This project is licensed under the EPL-2.0 License. See the LICENSE file for details.

Contact





Author: TOpPLUG



GitHub: https://github.com/TOpPLUG/Hubdarkweb



Discord: https://discord.gg/Hub7s

Join our Discord community for support, updates, and more Python tools!



Last updated: June 19, 2025
