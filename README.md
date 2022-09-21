# P1_Diego

This is a web API created to be consumed by other third-party applications that would allow users to view FIFA teams within a database, add a new team,
delete a team, view all players or by team, name, or position, trade a player from one team to another, add a player, and delete a player. This was written 
in C# using ASP.NET and ADO.NET. There are two controllers to separate the methods for FIFA teams and FIFA players along with classes for each. Additionally, as both would require 
properties from each other in order for the methods to work properly, I created an interface for FIFA players where I defined the appropriate properties,
had the FIFA teams class inherit that interface, and then had the FIFA players class inherit from FIFA teams. This allowed for both the parent and child class
to have access to the same properties without violating the Liskov Substition Principle. Here again, robust exception handling is implemented on both the client-side 
and the server-side so that users would recieve friendly and clear messages when they attempted to input incorrect information. 
