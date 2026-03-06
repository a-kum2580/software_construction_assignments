# Software Construction Research Assignment

## Overview
This research explores the concept of **Microservices Architecture** and how it is used by major technology companies. It also examines cases where companies moved back from microservices to **monolithic architecture**. The goal is to understand the advantages, challenges, and real-world applications of these software design approaches.

# 1. Microservices at Netflix

## Company: Netflix

Netflix is one of the most well-known companies using **microservices architecture**. Initially, Netflix operated using a **monolithic system**, but as the platform grew and began serving millions of users globally, the system became difficult to scale and maintain.

To solve this problem, Netflix transitioned to a **microservices-based architecture**.

### How It Works
In the Netflix system, the application is divided into **many independent services**, each responsible for a specific function. Examples include:

- User authentication
- Video streaming
- Movie recommendations
- Search services
- Billing and payments
- User profile management

Each microservice communicates with others through **APIs**.

### Why It Works Well for Netflix

Microservices allow Netflix to:

- **Scale services independently** depending on user demand
- **Improve reliability** since failure in one service does not crash the entire system
- **Enable faster development** because teams can work on different services simultaneously
- **Deploy updates continuously** without shutting down the entire platform

This architecture allows Netflix to support **millions of simultaneous streams worldwide**.


# 2. Other Companies Using Microservices

## Uber

Uber initially started with a **monolithic Ruby on Rails application**. As the company expanded globally and began handling millions of ride requests daily, the monolithic system became difficult to manage.

Uber migrated to **microservices architecture**, where different services handle different tasks.

### Examples of Uber Microservices

- Ride matching
- Driver management
- Payment processing
- Notifications
- GPS tracking

### Benefits for Uber

Microservices help Uber to:

- Handle **massive global traffic**
- Allow **different teams to work independently**
- Improve **system reliability**
- Enable rapid **feature development**

This architecture supports Uber's ability to process **millions of rides every day**.


## eBay

eBay is a large global online marketplace with billions of product listings and transactions. Originally, eBay relied on a **monolithic architecture**, which became difficult to maintain as the platform expanded.

To improve performance and scalability, eBay transitioned to **microservices architecture**.

### How Microservices Help eBay

eBay uses microservices to manage features such as:

- Product listings
- Search functionality
- Payment processing
- User accounts
- Recommendation systems

### Benefits for eBay

Microservices allow eBay to:

- Scale services during **high-traffic events**
- Improve system reliability
- Deploy updates without interrupting the whole system
- Support millions of buyers and sellers globally


# 3. Companies That Returned to Monolithic Architecture

Although microservices provide many advantages, some companies have experienced **high complexity and operational overhead**, leading them to return to **monolithic systems**.

## Amazon Prime Video Monitoring System

The Amazon Prime Video team built a **microservices-based system** to monitor video stream quality. The system analyzed streaming data to detect problems like glitches or synchronization issues.

However, the architecture became very expensive and complex because large volumes of data had to move between multiple services.

### Why They Switched Back

The team rebuilt the monitoring system as a **monolithic application** because:

- Communication between services increased costs
- Data transfers slowed system performance
- The system became difficult to debug and maintain

After switching back to a monolith, they **reduced infrastructure costs by about 90%** and improved performance.


## Segment (Twilio)

Segment is a customer data platform that previously operated with **over 150 microservices**.

Over time, this architecture created several challenges:

- Complex service dependencies
- Data consistency problems
- Increased maintenance overhead
- Slower development due to coordination between services

### Why They Returned to a Monolith

Segment simplified its architecture by consolidating services into a **monolithic system**, which helped to:

- Reduce operational complexity
- Improve system reliability
- Speed up development
- Make the system easier to maintain


## Conclusion

Microservices architecture has helped companies such as **Netflix, Uber, and eBay** build highly scalable systems capable of serving millions of users worldwide. By dividing large applications into smaller independent services, companies can improve scalability, reliability, and development speed.

However, examples such as **Amazon Prime Video's monitoring system** and **Segment** demonstrate that microservices are not always the best solution. In some situations, the complexity and operational costs of microservices may lead organizations to adopt **simpler monolithic architectures**.


## References

1. Netflix Technology Blog  
2. Uber Engineering Blog  
3. eBay Tech Blog  
4. Amazon Prime Video Engineering Blog  
5. Twilio / Segment Engineering Blog
