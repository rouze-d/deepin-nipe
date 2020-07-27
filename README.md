#### An engine to make Tor network your default gateway (for Deepin OS).

This tool is from:
<a href="https://github.com/GouveaHeitor/nipe"><h4>https://github.com/GouveaHeitor/nipe</h4></a>
by~ <a href="https://github.com/GouveaHeitor">Heitor Gouvêa</a> (Big thanks to you).

<p>However, the original nipe (<a href="https://github.com/GouveaHeitor/nipe">https://github.com/GouveaHeitor/nipe</a>) not working on Deeppin OS.<br>
So, I modified it a bit makes it work on Deepin OS.

<p align="center">
  <img src="https://heitorgouvea.me/images/projects/nipe/logo.png">
  <p align="center">An engine to make Tor Network your default gateway.</p>
  <p align="center">
    <a href="/LICENSE.md">
      <img src="https://img.shields.io/badge/license-MIT-blue.svg">
    </a>
</p>

---

#### How it works

    Tor enables users to surf the internet, chat and send instant messages
    anonymously,  and is used by a wide variety of people for both licit and
    illicit purposes. Tor has, for example, been used by criminals enterprises,
    hacktivism groups, and law enforcement  agencies at cross purposes, sometimes
    simultaneously.

    Nipe is a script to make the Tor network your default gateway.

    This Perl script enables you to directly route all your traffic from your
    computer to the Tor network through which you can surf the internet anonymously
    without having to worry about being tracked or traced back.
    
    Currently Nipe only supports IPV4, we are working on a solution to add IPV6 support and
    also only traffic other than DNS requests destined for local/loopback addresses is not passed
    through Tor. All non-local UDP/ICMP traffic is blocked.

#### Download and install on Deepin OS:
```
    # Download
    $ sudo apt install tor iptables iptables-dev
    $ git clone https://github.com/rouze-d/deepin-nipe
    $ cd nipe
    $ sudo cpan install Try::Tiny Config::Simple JSON
    $ sudo perl nipe.pl install
```

#### Commands:
```
    COMMAND          FUNCTION
    install          Install dependencies
    start            Start routing
    stop             Stop routing
    restart          Restart the Nipe process
    status           See status

    Examples:

    perl nipe.pl install
    perl nipe.pl start
    perl nipe.pl stop
    perl nipe.pl restart
    perl nipe.pl status
```

#### License

- This work is licensed under [**MIT License**](https://github.com/rouze-d/deepin-nipe/blob/master/LICENSE.md)
