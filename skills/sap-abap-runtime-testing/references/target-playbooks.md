# Target Playbooks

## SE38 report/program
Confirm selection-screen inputs, foreground/background behavior, messages, output type, variants, database effects, and termination conditions.

## Function module
Confirm import/export/changing/table parameters, update-task/RFC behavior, exceptions, commits, and side effects. Do not invoke update-enabled or posting functions automatically.

## Class/method
Confirm constructor/static state, method visibility, parameters, exceptions, persistence, and external calls.

## CDS/RAP/service
Static Reverse Engineer remains primary. Runtime Tester uses approved preview/service calls only through a separate safety decision and records filters, paging, user, and authorization context.
