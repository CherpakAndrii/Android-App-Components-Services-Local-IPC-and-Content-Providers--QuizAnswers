# Android-App-Components-Services-Local-IPC-and-Content-Providers--QuizAnswers
## Coursera quiz answers

* [Module 1(100%)](https://github.com/CherpakAndrii/Android-App-Components-Services-Local-IPC-and-Content-Providers--QuizAnswers#module-1)
* [Module 2(100%)](https://github.com/CherpakAndrii/Android-App-Components-Services-Local-IPC-and-Content-Providers--QuizAnswers#module-2)
* [Module 3(not ready)](https://github.com/CherpakAndrii/Android-App-Components-Services-Local-IPC-and-Content-Providers--QuizAnswers#module-3)
* [Module 4(not ready)](https://github.com/CherpakAndrii/Android-App-Components-Services-Local-IPC-and-Content-Providers--QuizAnswers#module-4)

# Module 1
### Question 1: Which of the following are ways in which the Layers pattern structures software apps and infrastructure (choose all that apply): 

* Provides services beyond the operating system and protocol stacks to enable components in a distributed system to communicate and manage data
* Enables end-to-end communication by specifying how data should be (un)packetized, addressed, transmitted, routed, and received
* ***Partitions an overall system architecture into groups of subtasks***
* ***Decomposes groups of subtasks into levels of abstraction***

### Question 2: Which of the following are reasons that layering is applied in Android (choose all that apply):    
* ***Reduces the complexity of APIs that app developers must understand***
* Increases context switching, synchronization, and data copying overhead
* ***Enhances systematic software reuse***
* ***Enables "plug and play" replacement of certain layer implementations*** 

### Question 3: Which of the following are implications of being "higher" in the memory hierarchy of a modern computing device (choose all that apply):

* ***Cost is greater***
* ***CPU access latency is lower***
* Memory bandwidth is slower    
* CPU access latency is higher    

### Question 4: Which of the following are correct statements of Android linux RAM (choose all that apply):    
* Apps running in user space can never access RAM of other apps
* ***Android Linux executes in kernel space RAM***
* User space is a less restrictive protection domain than kernel space    
* ***All Android apps execute in user space RAM***

### Question 5: Which of the following are true statements about Android's local and remote inter-process communication (IPC) mechanisms (choose all that apply):
* UNIX domain sockets are used to communicate with remote UNIX servers
* ***These IPC mechanisms reside within the kernel's device driver framework***
* ***TCP/IP is used to access the Internet***
* The Binder driver supports highly optimized LAN and WAN communication

### Question 6: Which of the following are true statements about processes in Linux (choose all that apply):    
* ***A process provides a unit of resource allocation and protection***
* ***A process contains one thread by default***
* A process provides units of execution for instruction streams that run on processor cores
* Processes appear at multiple layers in the Android software stack    

### Question 7: Which of the following are true statements about the Android Hardware Abstraction Layer (HAL) (choose all that apply):

* ***It shields higher layers of Android's software stack from Linux kernel idiosyncracies***
* It is implemented in kernel space to optimize performance and is written largely in C
* It's open source license ensures that all HAL driver implementations are available in open-source form
* It is implemented in user space and is written largely in Java    
* ***Android apps rarely access the HAL directly***
* ***It is implemented in user space and is written largely in C/C++***

### Question 8: Which of the following are true statements about the the "Android Runtime" (ART) execution environment that are not true for the Dalvik VM execution environment (choose all that apply):

* ***It provides a better garbage collector***
* It provides a Just-in-Time (JiT) compiler
* ***It provides an "Ahead-of-Time" (AOT) compiler***
* It executes standard Java Bytecode

### Question 9: Which of the following are examples of app components available in Android core libraries (choose all that apply):

* Phasers
* Threads
* ***Activity***
* ***Content Provider***
* ***Service***
* Stamped Locks

### Question 10: Which of the following are benefits of the Android Native Development Kit (NDK) (choose all that apply):

* ***It can help enhance performance by minimizing latency and maximizing throughput***
* It provides a managed runtime environment for executing Java garbage collection efficiently
* ***It can help integrate existing C/C++ libraries into Android apps***
* It can help improve portability across heterogeneous Java platforms

# Module 2

### Question 1: Which of the following are ways in which activities in Android are designed to be "ephemeral" (choose all that apply):

* ***They are destroyed and recreated to handle runtime configuration changes***
* They can interact with the user in powerful ways
* ***They are destroyed (and must be recreated later) when the back button is pressed***
* They perform long-duration operations and/or access remote resources via background threads/processes

### Question 2: Which of the following are types of Android services (choose all that apply):     

* Background services
* ***Scheduled services***
* ***Bound services***
* ***Started services***

### Question 3: Which of the following are examples of Android "hybrid" services (choose all that apply): 

* Alert service
* DownloaderService
* ***MusicPlaybackService***
* Activity Manager Service

### Question 4: Which of the following lifecycle hook methods apply to started services (choose all that apply):

* onUnbind()
* ***onDestroy()***
* ***onStartCommand()***
* onBind()
* onRebind()
* ***onCreate()***

### Question 5: Which of the following service lifecycle hook methods can be dispatched by Android when a bound service is in the "running" state (choose all that apply): 

* onCreate()
* onBind()
* onDestroy()
* ***onUnbind()***

### Question 6: Which of the following are examples of differences between the onCreate() and onStartCommand() hook methods of a started service (choose all that apply): 

* ***onStartCommand() receives the intent passed by the client that calls start service, whereas onCreate() does not***
* ***onCreate() is called once when startService() is first called, whereas onStartCommand() is called each time startService() is called.***
* onCreate() receives the intent passed by the client that calls start service, whereas onStartCommand() does not
* onStartCommand() is called once when startService() is first called, whereas onCreate() is called each time startService() is called

### Question 7: Which of the following are correct statements about the types of intents that can be used to create activities and services (choose all that apply):

* ***A service can be created via an explicit intent      
* ***An activity can be created via an explicit intent***
* ***An activity can be created via an implicit intent***
* A service can be created via an implicit intent

### Question 8: Which of the following are reasons why the MusicPlayer app is a simple example of a started service (choose all that apply):

* ***It doesn't need to spawn any internal threads explicitly***
* It runs the service in the same process as the activity
* ***There's no communication from the service back to the activity that invoked it***
* It is not started on-demand via the Activity pattern    

### Question 9: Which of the following are benefits of the IntentService framework (choose all that apply):

* It optimizes the scalability of concurrent services on multi-core hardware platforms
* ***It simplifies the creation of services that process requests concurrently***
* ***It doesn't require the complexity of the Model-View-Presenter pattern to handle runtime reconfiguration changes***
* It enables subclasses of IntentService to interact with the user in sophisticated ways

### Question 10: Which of the following explain the role of a deployment model in Android (choose all that apply):

* It makes it easy to run a service in the same thread or different threads
* ***It makes it easy to run a service in the same process or different processes***
* It directs the physical deployment of services to threads
* ***It directs the physical deployment of services to processes***

# Module 3
## Coming soon
