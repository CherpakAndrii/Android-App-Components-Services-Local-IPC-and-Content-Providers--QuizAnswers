# Android-App-Components-Services-Local-IPC-and-Content-Providers--QuizAnswers
## Coursera quiz answers

* [Module 1(100%)](https://github.com/CherpakAndrii/Android-App-Components-Services-Local-IPC-and-Content-Providers--QuizAnswers#module-1)
* [Module 2(90%)](https://github.com/CherpakAndrii/Android-App-Components-Services-Local-IPC-and-Content-Providers--QuizAnswers#module-2)
* [Module 3(100%)](https://github.com/CherpakAndrii/Android-App-Components-Services-Local-IPC-and-Content-Providers--QuizAnswers#module-3)
* [Module 4(100%)](https://github.com/CherpakAndrii/Android-App-Components-Services-Local-IPC-and-Content-Providers--QuizAnswers#module-4)

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

### Question 5: Which of the following service lifecycle hook methods can be dispatched by Android when a bound service is in the "running" state (choose all that apply): (?)

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

* ***A service can be created via an explicit intent***  
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

### Question 1: Which of the following are limitations with using startService() to communicate between an activity and a service (choose all that apply):
* ***startService() doesn't allow an extended "conversations"***
* startService() incurs security and performance drawbacks
* startService() does not allow extras to be passed with an intent in a consistent and useful manner
* startService() does not work across process boundaries

### Question 2: Which of the following are are unusual or disallowed use cases for activity and service communication (choose all that apply):

* Using a messenger to communicate from a service to an activity    
* ***Using startService() to communicate from a service to an activity***
* ***Using a messenger to communicate from an activity to a started service***
* ***Using a broadcast receiver to communicate from an activity to a started service***

### Question 3: Which of the following are limitations with using bindService() to communicate between an activity and a service (choose all that apply):

* ***bindService() does not allow extras to be passed with an intent in a consistent and useful manner***
* bindService() doesn't allow an extended "conversations"    
* bindService() incurs security and performance drawbacks
* bindService() does not work across process boundaries

### Question 4: Which of the following are correct statements about an Android handler (choose all that apply):

* ***A handler can be used to send and process messages in one or more threads within a single process***
* A handler can be used to send and process messages in one or more threads running in different processes
* A handler reference can be passed as data in a message or as an extra in an intent
* A handler can only run in the main thread of control in a process    
* ***A handler often eliminates the need for apps to use synchronizers***
* A handler implements the parcelable interface

### Question 5: Which of the following are correct statements about an Android messenger (choose all that apply):

* ***A messenger implements the parcelable interface***
* ***A messenger can be used to send and process messages in one or more threads within a single process***
* ***A messenger can be used to send and process messages in one or more  threads running in different processes***
* ***A messenger reference can be passed as data in a message or as an extra in an intent***

### Question 6: Which of the following are typical examples of what a started service does after it receives an intent from an activity (choose all that apply): 

* It returns a Binder reference to the activity via its onBind() hook method
* ***It obtains a reference to a messenger from the intent***
* It launches the service using the activator pattern    
* ***It returns results back to the activity via the messenger reference***
* It enhances in an extended conversation with the activity    
* ***It performs some processing***

### Question 7: Which of the following are correct statements about usage considerations for messengers (choose all that apply):

* Messengers are best suited for sophisticated interactions and complex data types
* ***App developers are responsible for marshaling and demarshaling of message content***
* Messengers shield app developers from marshaling and demarshaling details of message content
* ***Messengers are best suited for simple interactions and data types***

### Question 8: Which of the following is the behavior of the Android Activity Manager Service when the onStartCommand() hook method returns START_REDELIVER_INTENT (choose all that apply):

* It does not automatically restart the killed service, which must be explicitly restarted by an app
* ***It automatically restarts a killed service via a new call to onStartCommand() and supplies the same intent as was delivered this time***
* It communicates this return value back to the client activity
* It automatically restarts a killed service via a new call to onStartCommand() and supplies a null intent

### Question 9: Which of the following methods must be called to implement the Android "Concurrent Service Stopping" idiom (choose all that apply):

* onBind()
* onUnbind()
* ***onStartCommand()***
* ***stopSelf()***

### Question 10: Which of the following are correct statements about a bound service  (choose all that apply):

* ***A bound service lives only while it serves other app components***
* A bound service runs in the background indefinitely until the mobile device is powered down
* A bound service typically does not return a result to the activity that bound to it
* ***A bound service should be used when a client component wants to have an extended conversation with the service***

# Module 4

### Question 1: Which of the following are reasons why Android provides a content resolver class (choose all that apply):

* It defines a schema that represents a resource managed by a content provider
* ***It enables a content provider to be shared by multiple apps***
* ***It provides additional services, such as change notification***
* It stores data persistently in an SQLite database

### Question 2: Which of the following are operations supported on content resolvers (choose all that apply):

* ***bulkInsert()***
* ***insert()***
* bulkDelete()
* read()

### Question 3: Which of the following are actual behaviors of XML attributes that can be used to define a provider declaration in an AndroidManifest.xml file (choose all that apply):

* Indicate the task that the provider has an affinity for
* ***Designate if the content provider runs in a separate process or not***
* ***Grant permissions to allow other apps to read or write to the provider***
* List configuration changes that the provider will handle itself

### Question 4: Which of the following are terms that appear in the acronym "ACID" (choose all that apply):

* ***Atomic***
* Database    
* Concurrent
* ***Isolated***
* ***Durable***
* Asynchronous    
* Implicit    
* ***Consistent***

### Question 5: Which of the following are reasons why Android apps typically use concurrency or asynchrony when accessing an SQLite database (choose all that apply)

* Android filesystems are unreliable due to their use of flash memory
* ***Filesystem accesses are often relatively slow***
* SQLite doesn't support synchronous operations    
* SQLite supports the SQL92 specification, which is obsolete    

### Question 6: Which of the following are reasons why the SQLite query() method returns a Cursor (choose all that apply): 

* ***It is efficient since all data needn't be loaded into memory***
* It alleviates the need to explicitly call close() on the Cursor
* ***It allows buffering of query results***
* It ensures that query results work properly in concurrent programs    

### Question 7: Which of the following are reasons for using a content provider in an app (choose all that apply):

* To support user-facing operations in different configuration orientations
* ***To synchronize local data with remote data***
* To enable long-duration operations to execute in the background
* ***To offer complex data to other apps***
* To launch components on-demand in response to intents from other components
* ***To notify activities automatically when data changes***

### Question 8: Which of the following are parts of a content URI (choose all that apply):

* Metadata defining the synchronization policy for concurrent access
* ***An optional pa to an individual row in a table***
* ***The symbolic name of the provider***
* ***A na to a table or file***

### Question 9: Which of the following are motivations for content resolvers supporting content observers (choose all that apply):

* To designate rows and columns to return via a cursor
* To map content URI patterns to integer values using wildcard characters
* ***To avoid requiring apps from having to poll for updates to data storage***
* To initialize the associated content provider when it's first created

### Question 10: Which of the following are correct statements about why the HobbitActivity defines the HobbitOps class (choose all that apply):

* ***To consolidate and simplify operations on the HobbitContentProvider***
* To manage the persistent storage of Hobbit characters
* To create and manage the SQLite database    
* To define the metadata and schema for the SQLite database
