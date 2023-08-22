# Machine Config GitOps rollout

This project hosts 2 methods of rolling out Machine Config using GitOps.

The first method creates a job that will monitor `MachineConfigPool` status to ensure it updated all its `Machines`

The second method will pause the `MachineConfigPool` pool, apply the `MachineConfig` the resume the `MachineConfigPool`. This method is preferred when updating the `MachineConfigPool` where `ArgoCD Controller` is running.
