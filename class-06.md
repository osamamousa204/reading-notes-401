# HTTP Basics
HTTP allows for communication between a variety of hosts and clients, and supports a mixture of network configurations.

### URLs

Uniform Resource Locators (URLs).

consists of the following components:

`http://www.domain.com:80/assets/imgs?a=b`
- protocol : `http`
- host : `www.domain.com`
- port : `80`
- path to recource : `assets/img`
- query : `imgs?a=b`

### Verbs:
- `GET`: fetch an existing resource. The URL contains all the necessary information the server needs to locate and return the resource.
- `POST`: create a new resource. POST requests usually carry a payload that specifies the data for the new resource.
- `PUT`: update an existing resource. The payload may contain the updated data for the resource.
- `DELETE`: delete an existing resource.

**Method**                           | **Description**
-------------------------------------|-------------------------------------------
CONNECT                              | This specification reserves the method name CONNECT for use with a proxy that can dynamically switch to being a tunnel (e.g. SSL tunneling).
-------------------------------------|-------------------------------------------
DELETE                               | The DELETE method requests that the origin server delete the resource identified by the Request-URI.
-------------------------------------|-------------------------------------------
GET                                  | The GET method retrieves whatever information (in the form of an entity) is identified by the Request-URI.
-------------------------------------|-------------------------------------------
HEAD                                 | The HEAD method is identical to GET except that the server MUST NOT return a message-body in the response.
-------------------------------------|-------------------------------------------
OPTIONS                              | The OPTIONS method represents a request for information about the communication options available on the request/response chain identified by the Request-URI.
-------------------------------------|-------------------------------------------
POST                                 | The POST method is used to request that the origin server accept the entity enclosed in the request as a new subordinate of the resource identified by the Request-URI in the Request-Line.
-------------------------------------|-------------------------------------------
PUT                                  | The PUT method requests that the enclosed entity be stored under the supplied Request-URI.
-------------------------------------|-------------------------------------------
TRACE                                | The TRACE method is used to invoke a remote, application-layer loop-back of the request message.

![http](./img/http.png)

### What is REST

REST is acronym for REpresentational State Transfer. It is architectural style for distributed hypermedia systems and was first presented by Roy Fielding in 2000 in his famous dissertation.

Like any other architectural style, REST also does have it’s own 6 guiding constraints which must be satisfied if an interface needs to be referred as RESTful. These principles are listed below.

### Status Codes

**Overall range**                           | **Category**
-------------------------------------|-------------------------------------------
100-199                              | Informational
-------------------------------------|-------------------------------------------
200–299                              | Successful
-------------------------------------|-------------------------------------------
300–399                              | Redirection
-------------------------------------|-------------------------------------------
400–499                              | Client error
-------------------------------------|-------------------------------------------
500–599                              | Server error
-------------------------------------|-------------------------------------------

##### what i have learned 

HTTP stands for Hyper Text Transfer Protocol

WWW is about communication between web clients and servers

Communication between client computers and web servers is done by sending HTTP Requests and receiving HTTP Responses


[Home Page](https://osamamousa204.github.io/reading-notes-401/)
