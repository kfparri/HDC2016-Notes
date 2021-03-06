# HDC Notes

## Microservices - Morning session
 - Github location for source: [https://github.com/chaseaucoin/MicroDemo](https://github.com/chaseaucoin/MicroDemo "https://github.com/chaseaucoin/MicroDemo")
 - Decoupling is very important
	 - It allows you to change domains to something different to improve performance, such as changing from SQL Server to MongoDB
 - Testing
	 - You only test the service you are changing, not dependant services since they aren't changin.
 - Moving to this idea requires a culture shift
	 - Initial agility is slower
		 - Must ask the question "What domain does this service go to?"
	 - Large footprint, more services
		 - Must automate everything, testing deployment etc.
 - Similar to SOA
	 - Fewer components
	 - Logic across many domains
	 - Requires some form of Middleware
		 - Mulesoft, Corba, Biztalk
 - API Gateway
	 - Mashery
	 - Mulesoft
	 - Azure - API Gateway
 - Log Aggregation
	 - Stackify
 - Messaging
	 - RabbitMQ was his standard
	 - ZeroMQ with NETMQ
		 - Pattern and practices guides
		 - Really fast
 - Continuous delivery
	 - He recommends TFS..
	 - Octopus is one he mentioned
 - NuGet
	 - ProGet
	 - MyGet
	 - Nuget.Server
 - Multiple schemas in databases is a goo practice
 - 70% server load is the money spot
 - Failure as a service
	 - A service that randomly stops services and kills servers
	 - Keyhold Trouble Maker
 - Advanced installer and Update server
	 - Used to deploy to customers
 - He has a $1500 server farm!
	 - It looks like he's using Microsoft Azure Service Fabric
	 - AsRock BeeBox PCs with a load balancer and network switch.
		 - Each PC is running Windows Servers 2016
		 - To demo the fault tolerance I will need at least 3 PCs for a POC
 - 5 machines for fault tolerance in the Service fabric setup in class.
 - Swashbuckle.Core 
	 - Adds Swagger.io to a web API application.
 - Microsoft.Owin.Filesystems
 - Keyhole will do simple presentations on request.

## Afternoon Session
 - Protobuff? serialization.
 - Uses Microsoft's Memory Cache
	 - When scaling out, it can be just as good or better than Redis
 - Signal R
	 - .Net websockets.
 - Abstract and dissolve
	 - The process of moving legacy applications to the new paradigm
	 - Abstract the data manipulation then dissolve the old way of doing it.
 - Menagerie Gateway
 - 