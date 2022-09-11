# Microservices-SyncCommunication
Microservices Part1 - This is the first part of microservice series, example with synchronous communication between API Services.

This application contains 2 API which communicates with each other synchronously with http request.

The domin of the application is refered as warehouse management, where invertory comes in warehouse with orders and then it goes for quality check. After which the actual passed inventory will be considered as inventory inside warehouse.

So correcponsing the above scenario, this application contains two services as of now- 1) OrderService 2) QualityCheck Service.

The order service is used to have entries of order and order lines for new orders. Once the orders are added, then we can use createOrder method to send the
order for quality check.

It will call the quality check API via http call and create the entries for quality check.

As of not this application contains only 2 above mentioned services and will be upgraded in next parts.

This direct http call doesn't makes it a proper mircoservice, since in a microservice architecture one service doesn't depends on other and must be loosely coupled.

This will be done in next steps since its starting from scratch step by step.
