dmesg
Linux will show you the boot process logs during the boot. Some desktop systems hide this behind a fancy splash screen which you can hide using the Esc key or press Ctrl+Alt+F1.

In addition to these, most systems keep the boot logs in a text-like file too and they can be found in /var/log/boot or /var/log/boot.log in Debian or Red-Hat based systems, respectively.

init
When the Kernel initialization is finished, its time to start other programs. To do so, the Kernel runs the Initialization Daemon process, and it takes care of starting other daemons, services, subsystems and programs. Using the init system one can say "I need service A and then service B. Then I need C and D and E but do not start D unless the A and B are running". The system admin can use the init system to stop and start the services later.

systemd
Is new, loved, and hated. Lots of new ideas but not following some of the beloved UNIX principles (say.. not saving logs in a text file or trying to help you too much but asking for the root password when you are not running commands with sudo). It lets us run services if the hardware is connected, in time intervals, if another service is started, and ...

The systemd is made around units. A unit can be a service, group of services, or an action. Units do have a name, a type, and a configuration file. There are 12 unit types: automount, device, mount, path, scope, service, slice, snapshot, socket, swap, target & timer.

We use systemctl to work with these units and journalctl to see the logs.

We will speak more about runlevels on 101.3.