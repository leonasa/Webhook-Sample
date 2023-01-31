# Webhook2Kafka

## create a webhook
	| https://webhook.site/

## create a tunnel  
	| https://ngrok.com/
	| docker run -it -e NGROK_AUTHTOKEN=2L4kMfkMBzOdaXGdpHyIa31EC4a_2j11DLtdDjbb28o5xQLh9 ngrok/ngrok http 80
	| ngrok config add-authtoken 2L4kMfkMBzOdaXGdpHyIa31EC4a_2j11DLtdDjbb28o5xQLh9

## how to use tunnels
	| https://learn.microsoft.com/en-us/connectors/custom-connectors/port-tunneling
	| https://learn.microsoft.com/en-us/aspnet/core/test/dev-tunnels?view=aspnetcore-7.0

## worker
	| https://learn.microsoft.com/en-us/aspnet/core/fundamentals/host/hosted-services?view=aspnetcore-7.0&tabs=visual-studio

## install power platform tool (extension)
	| https://learn.microsoft.com/en-us/power-apps/developer/data-platform/tools/devtools-install

## best practices for webhook consumers
	| https://webhooks.fyi/

## create webhook in dataverse:
	| https://www.youtube.com/watch?v=d-aJYR6D8Og

## register a plugin
	| https://learn.microsoft.com/en-us/power-apps/developer/data-platform/register-plug-in

## webhook in dotnet
	| https://github.com/aspnet/WebHooks
	| https://khalidabuhakmeh.com/implement-a-webhook-framework-with-aspnetcore
	| https://github.com/damikun/trouble-training/blob/main/Doc/WebHookBackend.md

-----
-----
-----
### Api key 
| docker run -it -p 4040:4040 -e NGROK_AUTHTOKEN=token ngrok/ngrok:latest http host.docker.internal:5083
