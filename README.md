<p align="center">
  <img src="Images/tcqx-toolsV2-Banner.png" alt="tcqx-toolsV2-Banner" width="9999">
</p>

<h1 align="center">
  <img src="Images/tcqx-toolsV2-Logo.png" alt="tcqx-toolsV2-Logo" width="27">
  tcqx-toolsV2
</h1>

<p align="center">
  tcqx-toolsV2 is a multifunction tool dedicated to pentesting, OSINT and utilities.
  The project is open source and designed to centralize multiple security and
  information-gathering features into a single configurable platform.
</p>

<p align="center">
  <b>Version: v1.0 Beta</b>
</p>

<h2>⚠️ Disclaimer:</h2>

<p>
  This tool is intended exclusively for educational, authorized and lawful purposes.
  Only use the features against systems, websites, accounts or data for which you
  have explicit permission. The author is not responsible for misuse of this software.
</p>

<h2>📝 Description:</h2>

<ul>
  <li>⚙️ Compatible with Windows and Linux.</li>
  <li>🧠 Multifunction tool for authorized security testing and OSINT.</li>
  <li>🔎 Includes pentesting, reconnaissance and information lookup features.</li>
  <li>🛠️ Provides multiple scanning and analysis utilities.</li>
  <li>💻 Supports command-line usage.</li>
  <li>📄 Supports optional JSON output for several features.</li>
</ul>

<h2>📸 Preview:</h2>

<p align="center">
  <img src="Images/tcqx-toolsV2.png" alt="tcqx-toolsV2 Preview" width="9999">
</p>

<h2>⚙️ Installation:</h2>

<ol>

  <li>
    <b>Install the latest version of Python (3.14):</b>

    <br><br>

    <b>Windows:</b>

    <pre><a href="https://www.python.org/downloads/">Download Here</a> (The "PATH" option must be enabled during installation)</pre>

    <b>Linux:</b>

    <pre>sudo apt install python3 -y</pre>
  </li>

  <br>

  <li>
    <b>Install the latest version of Git:</b>

    <br><br>

    <b>Windows:</b>

    <pre><a href="https://git-scm.com/install/windows">Download Here</a> (The "PATH" option must be enabled during installation)</pre>

    <b>Linux:</b>

    <pre>sudo apt install git -y</pre>
  </li>

  <br>

  <li>
    <b>Clone the repository:</b>

    <pre>git clone https://github.com/tcqx/tcqx-toolsV2.git</pre>
  </li>

  <br>

  <li>
    <b>Enter the project folder:</b>

    <pre>cd tcqx-toolsV2</pre>
  </li>

  <br>

  <li>
    <b>Launch the setup:</b>

    <br><br>

    <b>Windows:</b>

    <pre>python setup.py</pre>

    <b>Linux:</b>

    <pre>python3 setup.py</pre>
  </li>

  <br>

  <li>
    <b>Launch the tool:</b>

    <br><br>

    <b>Windows:</b>

    <pre>python tcqxtools.py</pre>

    <b>Linux:</b>

    <pre>python3 tcqxtools.py</pre>
  </li>

</ol>

<h2>🔄 Update:</h2>

<ol>

  <li>
    <b>Enter the project folder:</b>

    <pre>cd tcqx-toolsV2</pre>
  </li>

  <br>

  <li>
    <b>Update the repository:</b>

    <pre>git pull</pre>
  </li>

</ol>

<h2>🚀 Features:</h2>

<pre>
Tools:
  --help            / -h  : Shows all tools options.
  --version         / -v  : Displays the version and information of the tool.
  --settings-update / -su : Update the tools settings.

  --mode            / -m  : Mode: decorated / interface
  --status          / -s  : Status: enable / disable


Pentesting:

  --advanced-scanner      / -as  : Advanced scanning performing all scans.
                                  (website, domain, IP, server)

    --target              / -t   : Service target:
                                  &lt;URL&gt; / &lt;domain&gt; / &lt;IP[:port]&gt; / &lt;localhost[:port]&gt;

    --output              / -o   : Creating additional JSON output.

    --http-timeout        / -HT  : Set the maximum HTTP timeout in seconds:
                                  &lt;timeout&gt;

    --socket-timeout      / -ST  : Set the maximum socket timeout in seconds:
                                  &lt;timeout&gt;

    --http-proxy          / -HP  : Set an HTTP proxy:
                                  &lt;proxy:port&gt;

    --socket-proxy        / -SP  : Set a socket proxy:
                                  &lt;proxy:port&gt;

    --useragent           / -u   : Set a user-agent:
                                  random / &lt;useragent&gt;

    --cookie              / -c   : Set a cookie:
                                  &lt;cookie&gt;


  --vulnerability-scanner / -vs  : Scan all vulnerabilities of a website.

    --target              / -t   : Website target:
                                  &lt;URL&gt; / &lt;domain&gt; / &lt;IP:port&gt; / &lt;localhost:port&gt;

    --output              / -o   : Creating additional JSON output.

    --http-timeout        / -HT  : Set the maximum HTTP timeout in seconds:
                                  &lt;timeout&gt;

    --http-proxy          / -HP  : Set an HTTP proxy:
                                  &lt;proxy:port&gt;

    --useragent           / -u   : Set a user-agent:
                                  random / &lt;useragent&gt;

    --cookie              / -c   : Set a cookie:
                                  &lt;cookie&gt;


  --port-scanner          / -ps  : Scan the ports of an IP.

    --target              / -t   : IP target:
                                  &lt;IP&gt;

    --mode                / -m   : Scan mode:
                                  single / multiple / range / default / all

    --port                / -p   : Port(s):
                                  single: &lt;port&gt;
                                  multiple: &lt;port&gt;,&lt;port&gt;
                                  range: &lt;port&gt;-&lt;port&gt;

    --protocol-scan       / -PS  : Protocol(s):
                                  TCP / UDP / TCP,UDP

    --output              / -o   : Creating additional JSON output.

    --socket-timeout      / -ST  : Set the maximum socket timeout in seconds:
                                  &lt;timeout&gt;

    --socket-proxy        / -SP  : Set a socket proxy:
                                  &lt;proxy:port&gt;


  --url-discovery-crawler / -udc : Scan all URLs of a website.

    --target              / -t   : Website target:
                                  &lt;URL&gt; / &lt;domain&gt; / &lt;IP:port&gt; / &lt;localhost:port&gt;

    --mode                / -m   : Scan mode:
                                  onlypage / allwebsite

    --output              / -o   : Creating additional JSON output.

    --http-timeout        / -HT  : Set the maximum HTTP timeout in seconds:
                                  &lt;timeout&gt;

    --http-proxy          / -HP  : Set an HTTP proxy:
                                  &lt;proxy:port&gt;

    --useragent           / -u   : Set a user-agent:
                                  random / &lt;useragent&gt;

    --cookie              / -c   : Set a cookie:
                                  &lt;cookie&gt;


  --ip-pinger             / -ip  : Continuously ping an IP.

    --target              / -t   : IP target:
                                  &lt;IP&gt;

    --mode                / -m   : Ping mode:
                                  ICMP / TCP

    --bytes               / -b   : Set the number of bytes for an ICMP ping:
                                  &lt;bytes&gt;

    --port                / -p   : Set the port for a TCP ping:
                                  &lt;port&gt;

    --interval            / -i   : Set the interval between each ping in seconds:
                                  &lt;interval&gt;

    --socket-timeout      / -ST  : Set the maximum socket timeout in seconds:
                                  &lt;timeout&gt;

    --socket-proxy        / -SP  : Set a socket proxy:
                                  &lt;proxy:port&gt;


  --host-discovery        / -hd  : Determines which hosts are online.

    --target              / -t   : CIDR target:
                                  &lt;IP&gt;/&lt;CIDR prefix&gt;

    --port                / -p   : Set the port for a TCP ping:
                                  &lt;port&gt;

    --output              / -o   : Creating additional JSON output.

    --tcp-icmp-timeout    / -TIT : Set the maximum TCP/ICMP timeout in seconds:
                                  &lt;timeout&gt;

    --socket-proxy        / -SP  : Set a socket proxy:
                                  &lt;proxy:port&gt;


OSINT:

  --dorking-query-engine     / -dqe : Query builder for Google, Bing and DuckDuckGo
                                      with advanced operators.

    --engine                 / -e   : Search engine:
                                      google / bing / duckduckgo


  --wallet-tracker           / -wt  : Track a crypto wallet's transactions with APIs.

    --address                / -a   : Wallet target address:
                                      &lt;address&gt;

    --output                 / -o   : Creating additional JSON output.

    --http-timeout           / -HT  : Set the maximum HTTP timeout for the API:
                                      &lt;timeout&gt;

    --http-proxy             / -HP  : Set an HTTP proxy for the API:
                                      &lt;proxy:port&gt;

    --useragent              / -u   : Set a user-agent:
                                      random / &lt;useragent&gt;


  --username-tracker         / -ut  : Track a username across multiple platforms.

    --target                 / -t   : The target username:
                                      &lt;username&gt;

    --output                 / -o   : Creating additional JSON output.

    --http-timeout           / -HT  : Set the maximum HTTP timeout in seconds:
                                      &lt;timeout&gt;

    --http-proxy             / -HP  : Set an HTTP proxy for the API:
                                      &lt;proxy:port&gt;

    --useragent              / -u   : Set a user-agent:
                                      random / &lt;useragent&gt;


  --email-tracker            / -et  : Track an email registered on several platforms.

    --email                  / -e   : Email target:
                                      &lt;email&gt;

    --output                 / -o   : Creating additional JSON output.

    --http-timeout           / -HT  : Set the maximum HTTP timeout for the API:
                                      &lt;timeout&gt;

    --http-proxy             / -HP  : Set an HTTP proxy for the API:
                                      &lt;proxy:port&gt;

    --useragent              / -u   : Set a user-agent:
                                      random / &lt;useragent&gt;


  --email-lookup             / -el  : Retrieve public data from an email.

    --email                  / -e   : Email target:
                                      &lt;email&gt;

    --output                 / -o   : Creating additional JSON output.

    --socket-timeout         / -ST  : Set the maximum socket timeout in seconds:
                                      &lt;timeout&gt;

    --socket-proxy           / -SP  : Set a socket proxy:
                                      &lt;proxy:port&gt;


  --ip-lookup                / -il  : Fetch public IP data using the ip-api.com API.

    --ip                     / -i   : IP target:
                                      &lt;IP&gt;

    --output                 / -o   : Creating additional JSON output.

    --http-timeout           / -HT  : Set the maximum HTTP timeout for the API:
                                      &lt;timeout&gt;

    --http-proxy             / -HP  : Set an HTTP proxy for the API:
                                      &lt;proxy:port&gt;

    --useragent              / -u   : Set a user-agent:
                                      random / &lt;useragent&gt;


  --phone-number-lookup      / -pnl : Retrieve public data from a phone number.

    --phone                  / -p   : Phone number target:
                                      &lt;number&gt;

    --output                 / -o   : Creating additional JSON output.


  --instagram-profile-lookup / -ipl : Retrieve public data from an Instagram username.

    --target                 / -t   : Username target:
                                      &lt;username&gt;

    --sessionid              / -s   : Your Instagram ID session:
                                      &lt;sessionid&gt;

    --output                 / -o   : Creating additional JSON output.

    --http-proxy             / -HP   : Set an HTTP proxy:
                                      &lt;proxy:port&gt;

    --useragent              / -u   : Set a user-agent:
                                      random / &lt;useragent&gt;


Utilities:

  --file-metadata-scanner / -fms : Scan all file metadata.

    --path                / -p   : The file path:
                                  &lt;path&gt;

    --output              / -o   : Creating additional JSON output.


  --file-metadata-deleter / -fmd : Remove all file metadata.

    --path                / -p   : The file path:
                                  &lt;path&gt;


  --website-cloner        / -wc  : Clone the entire web page.

    --target              / -t   : Website target:
                                  &lt;URL&gt; / &lt;domain&gt; / &lt;IP:port&gt; / &lt;localhost:port&gt;

    --http-timeout        / -HT  : Set the maximum HTTP timeout in seconds:
                                  &lt;timeout&gt;

    --http-proxy          / -HP  : Set an HTTP proxy:
                                  &lt;proxy:port&gt;

    --useragent           / -u   : Set a user-agent:
                                  random / &lt;useragent&gt;

    --cookie              / -c   : Set a cookie:
                                  &lt;cookie&gt;


Notations:

  /  : Or
  [] : Optional
  &lt;&gt; : Value
  *  : Required
</pre>

<h2>👨‍💻 Credits:</h2>

<ul>
  <li>Developed by: <b>tcqx</b></li>
  <li>GitHub: <a href="https://github.com/tcqx">github.com/tcqx</a></li>
  <li>GunsLol: <a href="https://guns.lol/tcqx">guns.lol/tcqx</a></li>
  <li>License: <b>MIT License</b></li>
  <li>Version: <b>v1.0 Beta</b></li>
</ul>

<h2>📜 License:</h2>

<p>
  This project is licensed under the
  <b>MIT License</b>.
</p>
