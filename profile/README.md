# Agents of the System

Turn your computer into an Agent! Smith will allow you to host private game servers with minimal effort directly on the machine you, likely, use most: Your gaming PC!  Later, find a crew, plug your programs into The Architect and share control over them.  Or, you can go it alone and use an Operator to directly interact with your agents.

Lost? Consult the Oracle for documentation and guidance.

## Motivation

A group of friends play various games like 7 Days to Die and VRising which require one of us to host a server
at our home.  We do this as opposed to paying for online hosting because this is a free options.  Often it's a hassle
to update a server or handle restarts of a server that might have gone down.  We have often mused over a tool that can
handle this workload for us or at least make it easier.  Also, a tool that doesn't require one of us to SSH into a home
server, Remote Desktop or have to require one of us to setup a home VPN. I have found similar tools that cost a lot of
money, or are open source and require one of us to be a tech expert to run it.  Nothing simple and in the middle.

I am creating a solution that follows a handful of simple principles:

1. Super simple to Use and runs on the machine you're used to working with.
2. A shared web application to group friends and game servers together.
3. Free for DIY types of people and cheaper for those that aren't.
4. Python Based Code base.

In short, the solutions I've seen run in a website or directly on a server.  Those solutions are great! Hats off to the
groups that built them.  My solution takes a distributed approach.  Think of it as a two part solution.  The first half of the solution will be a tool which runs on someones' local machine and has the ability to install game servers available via steam, start/stop servers, and do other similar tasks. I called that [AgentSmith](https://github.com/agentsofthesystem/agent-smith) because Agents are software tools that do things for us.  Smith because... you know.

For the DIY type person, I mentioned. There will also be a client and a minimal graphical user interface in the form of a system tray application.  I called the python client [Operator](https://github.com/agentsofthesystem/operator), because
an operator connects you, the individual, with Agent Smith.  The client and the agent, shall be able to communicate securely when performed outside of one's local network so not just anyone can interact with the agent.  People are free to use
the Operator for whatever purpose is desired.  AgentSmit and Operator are open source.

The other half of this solution is the shared web application, and that's being developed.  I cannot run that for free so at
this time its only something I'm willing to share directly with friends.  At some point, I would like to deploy it and charge
people enough to keep it running and make it worth my time to maintain.  I may chose to open source it at some point in the
future.  However, I called this part of the solution "The Architect", because an architect creates the system, tells the
agents in it what to do, and generally calls the shots.  Keep your eyes peeled in the [Projects](https://github.com/orgs/agentsofthesystem/projects) section for updates on how that is progressing.

## A word about licensing

I'll be completely honest, I'm worried that I'll open source my web application and find out that my hard work has been
copied and sold from under me.  Also that I'll lose control over its development in its formative phase.  So its closed
source for now.

But... AgentSmith, Operator and any documentation software will always be open source.  If you get use out of this tool and with to contribute back, please do.  You're welcome to use this software personally however you like.  However, I'm licensing AgentSmith with AGPL v3, and that means if you take this work and distribute it for personal gain, then you are lawfully required to make available all of your software. That include changes to this code base plus your own work.  There is also an obligation to provide a reference to this codebase and its [license](./LICENSE).  I gave Operator an MIT license so I, myself,
can use it in The Architect without having to share it back yet.

My motivation to do this stems from the idea that I truly wish this tool to be a community tool.  Even if I wind up building something that goes on to make me money, on some level I want it to be free to use for anyone with the skill, time and desire.  Also, I may also want my name on an open source tool that I created. Makes for good resume material!

## Acknowledgements

I do want to take my hat off to the people that built and maintain [Pterodactyl](https://pterodactyl.io/).  In a lot of ways,
it was an inspiration for me to build Agents of the System and go open source.

I also got a lot of inspiration from Kenneth Jiang who runs [Obico.io](obico.io), which is a 3D Printing tool that watches
prints and uses AI to detect failures.  At one point it was known as The Spaghetti Detective.  Ken's model for making software
open source and free for DIY types while also having a paid version is at the core of my aspirations.