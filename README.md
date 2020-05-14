# Rest - Best Practices and Conventions

# Whats?

## What is a Web Service?

## What is an API?

## What is REST?
* architectural style for distributed hypermedia systems
* Roy Fielding - "REST is a hybrid style derived from several of the network-based architectural styles and combined with additional constraints that define a uniform connector interface"

## REST vs SOAP
* REST is resource-oriented
* SOAP is action-oriented

# Representations
* JSON or XML is commonly used

# Richardson REST Maturity Model

## Level 0
* Using HTTP as a transport system for remote interactions
* Expose a service endpoint at some URI

## Level 1 - Resources
* Talking to individual resources

## Level 2 - HTTP Verbs

## Level 3 - Hypermedia Controls

# Conventions
## URLs

### Service root path

### Resources-oriented path

#### Plurals

## HTTP Responses
* 201 (Created)
  * POST
* 200 (OK)
  * GET
* PUT -> 
* DELETE -> 
* Errors
  * Http Status Codes
    * Client Errors
      * 400 (Bad Request)
        * When doing requests with a body which is not complaint with the one expected by REST API
        * Usually on field validations and body structure
      * 404 (Not Found)
        * When trying to access with GET (id), PUT or DELETE a specific resource which doesn't exist
      * 405 (Method Not Allowed)
        * When doing a request with a Http method that is not allowed or it doesn't exist
    * Server Errors
      * 500 - Internal Server Error - Generic One

# STOP versioning
* versioning leads to inconsistent and confusing endpoints
* versioning is hard to maintain
