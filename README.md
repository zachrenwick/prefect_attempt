# prefect_attempt

How to get started with prefect:
// not yet working
Commands:
- pip install prefect
- prefect backend server/cloud (you can change this at any time)
- prefect server start


if using cloud:
- prefect auth login --key <YOUR-KEY>


- run a flow?
- first create a project in cloud UI or use CLI with this command:
- prefect create project "first_project"

- before a flow can be run, you have to register a flow. This can be done in the flow python file using the command "flow.register"

- once the flow is registered under a project, it should show up in UI:
// link to picture here //

- pay attention to labels. this can help you specify which flows to run


next.. we can actually run the flow using cloud ui

to do this, you need to start a prefect agent.

agents can come from many different platforms (k8, ECS, docker, etc)


to run it locally:
- prefect agent local start

if you need to shut down the agent at any time, press control + c from command line

next we will execute a flow run. a flow run can be initiated from prefect cloud UI (probably easiest, just click "quick run" in top right corner)

it then uses the local agent to run the flow (even though you intiated it from cloud UI!)




