## Terrafrom cloud 

https://app.terraform.io/


Features:

1. Remote state storage - security, locking etc available
2. Private registry for modules
3. Integration with git-repos
4. Terraform runs in cloud
5. Variables and secrets management

Workflow options:

1. Remote execution mode:

    We can integrate a git repo with a workspace in HCP and set up a configuration where any update in git to trigger a workflow.

    We can setup following workflow,

    i.  Any pull request to main branch -> Trigger a speculative plan run

    ii.  On completion of merge request -> Trigger an "apply" run


2. Local execution mode:

    We can keep the workflow control in local or in a pipeline setup but keep the terraform state file in HCP platform.
