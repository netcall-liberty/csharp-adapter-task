# C# Adapter Task

## The Problem
This solution contains a simple `RefundService` that talks to different payment providers. `FakePayPalWebService` and `FakeWorldPayWebService` represent the live WorldPay and PayPal web services. These are simply ‘mock’ classes that demonstrate the functionality that the payment merchants offer.

In its current implementation, the `RefundService` is closely coupled to the (fake) third party services, which amongst other things makes the code long, potentially difficult to read, and not easily extendable or unit testable. The situation would only get worse over time as more and more payment providers are added.

## Your Task
One solution to this problem is to implement the Adapter pattern (see https://www.dofactory.com/net/adapter-design-pattern).

Our RefundService class is the Client in the adapter pattern and our FakeWorldPayWebService and FakePayPalWebService classes can be considered Adaptees. 
Your task is to refactor the RefundService class and add additional classes in order to implement this pattern. On completion of the task, the Client should no longer need to be aware of the underlying Adaptees implementation.

Add automated tests to validate your changes.


## Getting Started

1. Clone this repository

   ```bash
   git clone https://github.com/netcall-liberty/csharp-adapter-task.git
   cd csharp-adapter-task/src
   ``` 

2. Open `AdapterExample-v1.sln`
