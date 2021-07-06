<!-- classes: title -->

# 🔧 How to build modern web apps?

### Prashanth Gandhiraj
<!-- block-start: grid -->


<!-- account: twitter, your-account-name -->
@neotheicebird
<!-- block-end -->
📧 prashanthgandhiraj@gmail.com

---

# About me

- 🧑‍💼I run a Freelance business 
- 👨🏽‍💻 Full stack developer 
- ♟️ Casual Chess player 
- 🍿 Recently turned Binge-watcher

<!-- note


-->
---
# What can you expect from this talk?


- What kind of problems can we solve using web Applications?<br/><br/>

- How were web applications made in the past?<br/><br/>

- How are they made nowadays?<br/><br/>

- How you can start developing one today!<br/><br/>


---

# What are web applications?

Let's create a conceptual understanding:-
<br/>

- An ✨Application✨ is a type of software<br/><br/>

- Helps humans achieve a task ✔️<br/><br/>

- Reduce human effort<br/><br/>

- Can create new Possibilies and Expand human consciousness 🌌

<!--note 
Take for example an app like Facebook. It has connected human beings across the world and this improved communications has fundamentally changed how we look at life.
-->
---

# What are web applications?


---

# What are web applications?

- A ✨Web Application✨ is an application that is accessible "online"<br/><br/>

- It has atleast two components, a client and a web server<br/><br/>

- client handles human interactions<br/><br/>

- A server protects resources and handles business logic<br/><br/>

- Client and Server use Web Protocols to communicate


---

# Web Applications: Examples 📱

- Travel: Ola, Metro Train App

- Communication: Whatsapp, Discord, Zoom

- Food: Swiggy, Big Basket

- Shopping: Amazon, Myntra

---

# They are everywhere!

![TheyAreEverywhere](https://media.giphy.com/media/p9G0FYn3Wr1Tjz7VbL/giphy.gif)

<!-- note
Not just consumer apps, there are enterprise apps which are used by employees to help them work better.
-->

---

# But how did we get so good at making them?

## 🤔

---

# But how did we get so good at making them?

- Years of created software assets, documented best practises and ever active software community<br/><br/>
- Its a long standing experiment<br/><br/>
- The industry has mutated and better traits emerge as trends<br/><br/>
- Open Source Culture 💖

<!-- note
But how did we get so good at making them?

Like any other discipline, through years of practise and by making multiple iterations, the craft of making web apps is now at a peak never before.

Right now, So much of that wealth of decades of work is available for us to use and realize so many of our ideas!
-->

---

# Basic Structure of a Web Application

<!-- block-start: grid -->

<!-- block-start: column -->
![Client-server-model.svg](./assets/Client-server-model.svg)
<!-- block-end -->
<!-- block-start: column, left -->
- Client has the human computer interface<br/><br/>
- Server does tasks, Protects and Handles resources<br/><br/>
- A network connects Clients with the server

<!-- block-end -->

<!-- block-end -->
...

---

# Key aspects of apps made in the past?

- Dynamic, on the fly HTML<br/><br/>
- Usage of a variety of databases<br/><br/>
- 🤹🏻‍♂️ Complex systems that solved many problems<br/><br/>
- like skyscrappers, Vertically structured<br/><br/>
- Deeply coupled features 🙀

<!-- note
While it would take long to explore the entire history of software development, lets try to understand the last generation and its downsides before we understand where we stand now.
-->

---

# Some Problems solved by web servers

- Properly route and parse requests
- Data Storage
- Authentication and Authorization
- Scheduling and Backend Tasks
- Server static assets and frontend code

---
# Some issues with the past architectures

- Improper Segregation of Responsibilites = More Bugs, Harder Maintenance
- Single Point of Failure
- Difficult to Scale
- Bigger bills and lesser fuel for creativity

---


# Trying too many things at once

![DoingTooManyThings](https://media.giphy.com/media/DcCcyWVDeKMec/giphy.gif)

---

# Monolithic Architecture

![Monolith](https://upload.wikimedia.org/wikipedia/commons/thumb/0/01/Card_castle6.JPG/220px-Card_castle6.JPG)

<!-- note
Stacked on top of one another, the system is not stable often and not very scalable.
-->
---

# Monolithic Architecture

Roles:

1. Software Developers
2. Operation Specialists

<!-- note
Software Engineers and Operations/Information Technology (Ops/IT) Specialists. Software engineers were responsible for writing code to solve a customer problem. Once the code was ready, an Ops/IT professional would deploy it to production servers and monitor it to ensure everything was running smoothly
-->
---


# How is the ecosystem different today?

- The drawbacks of monolithic architecture inspired many experiments<br/><br/>
- The main emergent trend is the "services" model of solving applications

---

# What are Services?


- Services are softwares that take up a single responsibility and does it really well
- Thinking about app as a set of services
- We don't have to solve everything by hand<br/><br/>
- Delegate responsibilities and Trust these services

<!-- note
Instead of spending our resources into whats been solved already, if we can cooperate and work together, we achieve more. We can also easily focus on the problem we are trying to solve.
-->

---

# Services: Examples

- Authentication: [Auth0](https://auth0.com/), [Cognito](https://aws.amazon.com/cognito/)
- Email: [Mailchimp](https://mailchimp.com/), [SendGrid](https://sendgrid.com/)
- Data Storage: [MongoDB](https://www.mongodb.com/), MySQL instance in AWS
- SMS, Phone Calls: [Twilio](https://www.twilio.com/)
---

# Services: Examples

- Business Logic: [AWS EC2](https://auth0.com/), [Digital Ocean](https://aws.amazon.com/cognito/)
- Payment: [Razorpay](https://razorpay.com/), [Stripe](https://stripe.com/en-in)

<!-- note 

Breaking up applications into "services" is the central idea in the process of today's app development - If you take the analogy that a system (like uber) is like an organism (like human body), then its made of organs each performing a set of tasks its aware of. 

But there emerges a synergy, a natural intelligence, that keeps everything working together.

-->
---

## How to build a Web App that can make use of these services?

---

# Event-based Microservices Architecture

Its an architecture style in which we connect a collection of services, such that they are: <br/><br/>

- Highly maintainable and testable
- Loosely coupled
- Independently deployable
- Organized around business capabilities
- Owned by a small team

---
# Microservices Architecture

![microservices](https://microservices.io/i/Microservice_Architecture.png)

<!-- Note 

Your business logic can be split into many decision making units.
In monolithic arch, we see your logic as one unit, because if it went down, the entire server is down. 

But here think like many servers are deployed and each taking care of one responsibility.
-->

---

# How does our Application Connect to services?

- APIs - To delegate tasks
- Web Hooks - To respond to events

---

# APIs

An API is an ✨Application Programming Interface✨

- Software interface to help one software talk to another
- Popular usage of APIs in Web Apps are RESTful APIs
- Other protocols are RPC
- Tech that goes with APIs: GraphQL, SDKs

---

# APIs

![buttons](https://media.giphy.com/media/9DavVitIZ26jH0aK7s/giphy.gif)

<!-- note 
Your software is going to talk to another software like pressing buttons.

-->
---

# API Example: Twilio

<!-- block-start: grid -->

<!-- block-start: column -->

```python
from twilio.rest import Client

# Your Account SID from twilio.com/console
account_sid = "ACXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX"
# Your Auth Token from twilio.com/console
auth_token  = "your_auth_token"

client = Client(account_sid, auth_token)

message = client.messages.create(
    to="+15558675309", 
    from_="+15017250604",
    body="Hello from Python!")

print(message.sid)
```
<!-- block-end -->
<!-- block-start: column, left -->
Using Twilio SDK, which uses the Twilio REST API, we are sending a message to a phone.

<!-- block-end -->
<!-- block-end -->

<!-- note 
Your software is going to talk to another software like pressing buttons.

-->
---

# Web Hooks

Web Hooks are event listeners you add to your application.

Sometimes users interact with the services directly, in such cases, the services can let your application know about an user event through Web Hooks.

---

# Example of Web Hooks: MailChimp

<!-- block-start: grid -->

<!-- block-start: column -->

```json
{
    "key": "YOUR_API_KEY",
    "url": "http://example.com/webhook-url",
    "description": "My Example Webhook",
    "events": [
        "send",
        "open",
        "click",
        "hard_bounce",
        "spam"
    ]
}
```
<!-- block-end -->

<!-- block-start: column, left -->

When your Mailchimp Transactional account recieves an user reply OR any other event occurs, mailchimp can pass on that information to your app by "hitting" your web hook.

<!-- block-end -->

<!-- block-end -->

<!-- Note 
With APIs and Web Hooks our application can establish 2-way communication with services.

-->
---

# Two Pillars of Microservices

1. Serverless
2. Containers

---

# Serverless

- Mostly refers to FaaS (Functions as a Service)
- Popular providers are AWS Lambda, Azure functions, Google Cloud Functions, IBM FaaS


---

<!-- section-title: Bye👋 -->


## Bye👋

<!-- block-start: grid -->


<!-- account: twitter, your-account-name -->
@neotheicebird
<!-- block-end -->
📧 prashanthgandhiraj@gmail.com
