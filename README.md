**Horizen.FullNode.API.Net.Standard**

Author: [PeaStew](https://github.com/PeaStew)

Contributors:
 - none

This repository contains a .NET Standard 2.1 library for use with any .NET projects to allow connection to a Horizen full node ([zend](https://github.com/HorizenOfficial/zen)) via RPC. It uses JSON RPC 2.0 which allows batching of commands and makes use of Generics to simplify the RPC call process.

As this library has the potential to cause loss of funds due to a programming error in the library itself or by mistakes made by the user when using the library in an application, it is released with any warranty of any kind in accordance with the MIT licence under which it is released.  

**USE AT YOUR OWN RISK.**

There are some known limitations with this library which will be improved over time and updated in this README when they have been fixed:
 - Currently omits the RPC calls related to mining (this is a priority to complete)
 - Currently omits the new Sidechain related calls (this is due to the immaturity of those functions, when they are declared final by the zend and zend_oo SDK authors then they will be implemented)

Other things that are on the list of improvements list:

 - [ ] Introduce the [ZMQ](https://github.com/ZencashOfficial/zen/blob/master/doc/zmq.md) and [AMQP](https://github.com/ZencashOfficial/zen/blob/master/doc/amqp.md) capabilities to allow streaming of data from the zend process for use in explorers for example.
 - [ ] Improve the call stack to avoid the current necessity to direct calls to underlying functions is specific cases
 - [ ] Improve the commenting within the application to help describe the logic, for the most part the application is very simple and shouldn't require too much description as it merely abstracts the RPC calls process that is available from the built in help in the zend application itself, nonetheless in the spirit of being a good coder, it will be done... eventually.
 - [ ] Release the library on nuget so it can be used within an application without needing to build it as part of the project.

Contributions are extremely welcome on this library, I have done this in my free time up until this point and have used this in many personal applications as well as for projects for Horizen, for example [notes.horizen.global](https://notes.horizen.global) which combines Blazor Serverside with this library to show the messages on the Horizen mainchain in the null_data field.

Enjoy!

PeaStew
