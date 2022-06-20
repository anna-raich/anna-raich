# <Microservice Name>

<*Description: what a service delivers, providing an informative, descriptive, and comprehensive overview of the value that this microservice brings.*>  
Example: *This service is used to obtain information about the working permits debts info and display it to the user.  
User can try to generate SADAD number for `debt id`.*

Take a look at the components diagram that describes them and their interactions.  
<*Diagram here*>

## IBM Endpoints Workflow

IBM endpoints used by this microservice are as follows (click on the endpoint name to view its documentation with request and response examples):  
*<Example endpoints>:*  
- [get wp debt info](https://employeesgate.atlassian.net/wiki/spaces/QI/pages/3827073379/Get+Establishment+WP+Debit+Info+-+ISD)
- [generate sadad number](https://employeesgate.atlassian.net/wiki/spaces/QI/pages/3828056157/MLSD+GenerateWPDebitSadadNo+-+ISD)

*<If a microservice requires a certain flow of working with IBM endpoints, include a description of the flow.>*

## HTTP Verbs
List of the relevant HTTP methods with descriptions and their respective URLs.  
*<Example HTTP methods>:*  
| HTTP METHOD | URL                    | DESCRIPTION                             |
|-------------|------------------------|-----------------------------------------|
| GET         | /company-est-balance   | Retrieve working permits debts from IBM |
| POST        | /sadad-number/generate | Generate SADAD number for debt id       |

## Service Logic
Technical description of this microservice's logic.  
Example: *According to the IBM response service parses JSON and setups establishment type and needed fields after it service returns serializable data on the FE.*

## Requirements
- Ruby 2.7.1
- RabbitMQ
- Redis

## Configuration
### RabbitMQ
<URL>  

### Redis
<(Session) URL>  

### IBM settings
<Keys, secret, errors, url, auth>  

### Settings for FE
<Virtual host and virtual port>  

### Airbrake settings
<Airbrake settings>  

### Env variables
<Currently used env variables>

## Testing
<How to run tests>  

## Troubleshooting
- Monitor the performance of the IBM endpoint (check via `mlsd.sh`)
- Make sure that all the variables are configured correctly
