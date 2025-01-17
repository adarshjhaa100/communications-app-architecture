# Learn software development the fun way: Build a communcations app from scratch 

### Prerequisites: Should have basic knowledge of atleast one programming language. If not I recommend atleast complete a basic crash course first.

Want to learn a new language in a fun way? Want to become a better developer doing that? Let's build a communications app starting with the description provided. 

By the time we finish building this, we'll be able to understand in depth the implementation the following concepts and technologies:

- Backend Communcation Protocols
- GUIs/CLIs
- File Storage
- Databases
- Data Strctures and Algorithms: Trees, String, Search etc. 
- Video/Audio Processing
- String processing
- File handling
- Image Processing
- DevOps: Build, Deploy and Diagnostics
and much more...


Google, use UI or do whatever you want to search whenever stuck. Just make sure to properly understand if copying any code, using library, tools etc. happy coding!


#### User Requirements: 

- Send chat to A chatgroup ( 1 or more people ).
- Persist chat (for a specific chatroom and visible to subscribed user)
- Chat format: text, file(preview options for image), URL
- Audio/Video Calling, WIth screen sharing
- Browse the chat history, groups, call history etc.
- with GUI
- Settings, Call History etc.
- Chat backup and Migration Options
- Embed social media feature. Turn chats/images/videos into social media style
- <b>App Should Work on : Mobile, Web and Desktop (Can make three different versions)</b>
- Screen Sharing


#### Technical Requirements:

- Follow these steps for an effective learning: Go over the topics of a language at a high level -> Create a mind map -> Write hello world (Lol!) ->Start building (or if it's tough, do AOC) -> Keep using mindmap to search whenever you want to use something -> Post solution, compare with industry level code (Maybe from open source) implementing the same and check for any improvements in your code.

- Languages : JS,Go, Python, C, Java, Rust, Zig or whatever you'd like to use. Just use any one across whole application for understanding the nuances.
- Files, chats can be compressed
- Identify how each tool’s (language, library, Framework) used across the industry.
- App Should Work on : Mobile, Web and Desktop (Can make three different versions)
- Figure out error handling in whatever tool being used to build this. Try to add failure recovery mechanisms if possible.
- A small tip here: try to convert small parts of your code to assembly/obj/bytecode. Search the internet if anything seems foreign and keep on going.
- Try to be less dependent on third party libraries, only use when absolutely required. If you really use something, try to understand the internals, explore code etc,
- <b> Setup Benchmark, Testcases, Fuzzing, Dockerize, Build and Deployment Scripts, Diagnostics (Logging, Metrics, Audit, Debugging etc.) from the get go to get a full picture </b>
- <b> Use benchmark and profiling results to optimize the most longest running pieces of codes. View the bytecode, assembly, memory representation of data during runtime, etc. </b>
- <b> Feature flag and env flag for prod, dev etc.  if env = dev then only run diagnostics </b>
- Try to improve the application to squeeze out every last bit of performance.
- Once the initial prototype is complete, try deploying it over some free tier linux server, or any cheap linux service provider. Automate deployment by installing tools like jenkins(or use github workflows) on your local machine.
- Research on the best security practices used across the industry and try applying those relevant to the application.
- Go over webrtc: [https://webrtc.github.io/webrtc-org/architecture](https://webrtc.github.io/webrtc-org/architecture/#), understand architecture and try building a rough one of your own using udp/tcp

#### Document Every significant detail of the technical decisions and designs, taken throughout. Discuss tradeoffs if exists, and try to do a comparison with other existing techniques. Some examples:
- Constraints, Requirements
- Platform: Client and Server. Mobile? Web? IOT? etc.
- High Level and Low level architecture based on the tradeoffs and decisions
- Decision on: Service logic, Data-Storage, Communication (e.g RPC for internal, client server for external, Message Queues)
- Fault Tolerance Mechanisms: Reliability, Availability, Safety, Maintainability
- Using any specific mechanism like: cache? Message Queues? Why? what is the complexity, cost and benefit for the usage.
- Diagnostics information
- Benchmark and usage patterns
- <b> In the end, the purpose is to iteratively improve the software based on the information </b>  



#### Rough Guidelines For Benchmarks:
- <b>Idea Here is to squeeze out the best performance with available resources. Keep going on until resource usage hits bottleneck, then improve, and keep on repeating the cycle. Reasearch on optimization techniques in whatever tool you're using</b>
- 1. Notice the Spike in resource usage. 2. Identify The component/function/process taking the most amount of time for this.
- Send and Store the following no of text messages: 10K, 100K, 1 million, 10 million and so on. (spread across multiple groups and users)
- Send files worth: 1 MB, 10 MB, 100 MB and so on
- The following number of calls at a time across the application space: 1000, 10k, 100k and so on etc.
-  <b> Use benchmark and profiling results to optimize the most longest running pieces of codes. View the bytecode, assembly, memory representation of data during runtime, etc. </b>


## UI SCREENS:

***Login:***

![image](https://github.com/adarshjhaa100/communications-app-architecture/assets/31096082/f5823003-a0cb-4b47-a09b-e7849138e9d5)


***Chat:***

![image](https://github.com/adarshjhaa100/communications-app-architecture/assets/31096082/2a6903fe-39d1-4115-bf44-1ca3e097b52b)


***Search:***

![image](https://github.com/adarshjhaa100/communications-app-architecture/assets/31096082/962ddea6-23e1-40b9-8e78-75d19512b6ce)


***Call:***

![image](https://github.com/adarshjhaa100/communications-app-architecture/assets/31096082/53acaa4c-c490-45ac-bf4d-46c5aa88fdf8)


## ARCHITECTURE

Note: The architectures mentioned here are just a suggestion. Implement this if you'd like, or design something and create a PR!

Try to build a basic version of bidirectional communication (Like WebRTC), or Just use webRTC,webSocket and look at the inner workings of whatever library used.

For UI, Use the most basic lib/framework available (Desktop: QT, SDL, GTX etc. , Web: PureJS, integrated with WASM if possible), Understand how they works in depth.


**High Level Frontend Arch**


![image](https://github.com/adarshjhaa100/communications-app-architecture/assets/31096082/8ce6ac8d-0869-470a-8706-fab13aee3fb3)


**High level Backend API**

![image](https://github.com/adarshjhaa100/communications-app-architecture/assets/31096082/3a4f9abf-f2cf-426d-9af4-ebf345b8793b)


Do reach out or raise a PR for any suggestions.

