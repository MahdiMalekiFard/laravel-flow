<h2 align="center" style="color: yellow;">( General Documentation )</h2>

## <span style="color: lightblue;">What is a workflow?</span>

#### Two concepts define a workflow in team-managed projects:
>1. <b style="color:green;">Statuses</b> - the steps in your team’s working process that describe the state of a task.
>2. <b style="color:green;">Transitions</b> – how a piece of work can move between statuses.


## <span style="color: lightblue;">What are workflow statuses?</span>
>Statuses help people understand the state of a piece of work.
They appear in many views across your site.


[flow-status]: ../../images/flowStatuses.png
[![product-screenshot][flow-status]](https://example.com)

## <span style="color: lightblue;">What are workflow transitions?</span>
>Transitions connect statuses and help define the flow of work in your project.


[flow-transition]: ../../images/flowTransitions.png
[![product-screenshot][flow-transition]](https://example.com)

>These pathways define how people move pieces of work through your workflow.
For example, if you run a pizza shop, you might have different statuses depending on who’s picking up the pizza.
Once the pizza is “Ready for pickup”, it can move down the “Send for delivery” transition, putting it in the “On the way” status.
Or, it can transition down the “Give to customer” transition, showing that the pizza work is done.


## <span style="color: lightblue;">What are workflow Tasks?</span>
>When the flow goes from one state to another through a transition some tasks will be executed like sending sms or calculating a mathematical operation ...
There are two kinds of tasks: Global and Asset-related-Tasks.


## <span style="color: lightblue;">What are workflow Assets?</span>
>We have an assetable morph field that allows you to define different types of assets like loan requests and payments ... . This asset will be 
placed in a state where a user should make decisions about it and the status of the state will be changed and the request goes to the next state.


## <span style="color: lightblue;">What is a Driver?</span>
>A driver is a class that has different methods and properties with a handle method that allows you to run it.


## <span style="color: lightblue;">Conclusion</span>
>With this package you can create a flow which has a driver for itself and can be active or inactive depending on the status of the flow. For example, you 
have the Loan flow which has LoanFlowDriver. for this Loan flow you can create several flow-states which the first one must have the **START** status.
flow states are connected to each other by flow-transitions and alongside the flow-transition some tasks can be executed. Each flow-task has its own driver.
you can see the list of all flow-task drivers. there are global tasks that are mentioned in the list.

>When each of flow related parts stored or updated an event will be called, and you can use that for different purposes.
