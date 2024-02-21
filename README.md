# Running-Notes
## API Management : 
https://learn.microsoft.com/en-us/azure/api-management/api-management-key-concepts
#### API Management Componenets
Azure Api Management is made up of an API Gateway, a management plane and developer portal. 
Thease components are azure-hosted and fully managed by default.
API Management is available in verious tiers diffring in capacity and features.

![image](https://github.com/venurao/Running-Notes/assets/19890397/2e36bdbb-4a76-4999-8f5e-eeb1b9938e84)

### API Gateway
All requests from client application first reach API Gateway, which then forwards them to respective backend services.
They API acts as facade to the backend services, allowing API providers to abstract API implementations and evolve backend architecture without impacting API consumers.
The gateway enables consistent configuration of routing, security, throttling, cahching and observability<br/>

- Acts as a facade to backend services by accepting API calls and routing them to appropriate backends.<br/>
- Verifies API keys and other credentials such as JWT tockens and certificates presented with requests.
- Enforces usage quates and rate limits
- Optionally transforms requests and responses as specified in policy statements.
- if configured, caches responces to improve latency and minimize the load on backend services.
- Emits logs,metrics, and traces for monitoring, reporing and troubleshooting.

