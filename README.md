# Threat-Modeling


Scenario : -

You’re part of the growing security team at a company for sneaker enthusiasts and collectors. The business is preparing to launch a mobile app that makes it easy for their customers to buy and sell shoes. 

You are performing a threat model of the application using the PASTA framework. You will go through each of the seven stages of the framework to identify security requirements for the new sneaker company app.


                                                                        PASTA FRAMEWORK STAGES


Step 1 : - Identify the mobile app's business objectives :

The main goal of Stage I of the PASTA framework is to understand why the application was developed and what it is expected to do.

Description : -  Our application should seamlessly connect sellers and shoppers. It should be easy for users to sign-up, log in, and manage their accounts. Data privacy is a big concern for us. We want users to feel confident that we’re being responsible with their information.

Buyers should be able to directly message sellers with questions. They should also have the ability to rate sellers to encourage good service. Sales should be clear and quick to process. Users should have several payment options for a smooth checkout process. Proper payment handling is really important because we want to avoid legal issues.


Step 2 : - Evaluate the app's components

In Stage II, the technological scope of the project is defined. Normally, the application development team is involved in this stage because they have the most knowledge about the code base and application logic. Your responsibility as a security professional would be to evaluate the application's architecture for security risks.

For example, the app will be exchanging and storing a lot of user data. These are some of the technologies that it uses:

Application programming interface (API): An API is a set of rules that define how software components interact with each other. In application development, third-party APIs are commonly used to add functionality without having to program it from scratch.

Public key infrastructure (PKI): PKI is an encryption framework that secures the exchange of online information. The mobile app uses a combination of symmetric and asymmetric encryption algorithms: AES and RSA. AES encryption is used to encrypt sensitive data, such as credit card information. RSA encryption is used to exchange keys between the app and a user's device.

SHA-256: SHA-256 is a commonly used hash function that takes an input of any length and produces a digest of 256 bits. The sneaker app will use SHA-256 to protect sensitive user data, like passwords and credit card numbers.

Structured query language (SQL): SQL is a programming language used to create, interact with, and request information from a database. For example, the mobile app uses SQL to store information about the sneakers that are for sale, as well as the sellers who are selling them. It also  uses SQL to access that data during a purchase.



Step 3 : - Review a dataflow diagram

During Stage III of PASTA, the objective is to analyze how the application is handling information. Here, each process is broken down.

For example, one of the app's processes might be to allow buyers to search the database for shoes that are for sale. 


Step 4 : - Use an attacker mindset to analyze potential threats

Stage 4 is about identifying potential threats to the application. This includes threats to the technologies you listed in Stage 2. It also concerns the processes of your data flow diagram from Stage 3.

For example, the apps authentication system could be attacked with a virus. Authentication could also be attacked if a threat actor social engineers an employee.


Step 5 : -   List vulnerabilities that can be exploited by those threats 

Stage 5 of PASTA is the vulnerability analysis. Here, you need to consider the attack surface of the technologies listed in Stage 2.

For example, the app will use a payment system. The form used to collect credit card information might be vulnerable if it fails to encrypt data.


Step 6 : - Map assests, threats, and vulnerabilities to an attack tree

In Stage 6 of PASTA, the information gathered in the previous two steps are used to build an attack tree.

Step 7 : - Identify new security controls that can reduce risk

 In Stage 7, the final goal is to implement defenses and safeguards that mitigate threats.

