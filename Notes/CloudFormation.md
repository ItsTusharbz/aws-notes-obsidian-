Infra as code
- no resources are manually created, excellent for control.
- Changes to the infra are reviewed through code.

Cost
- Each resource within stack is tag so that it can be identified for the cost.
- you can estimate the costs of your resources using cloudFormation template.
- Saving strategy: in Dev you can schedule deletion and creation based on need. (eg create 8 AM and delete at 8 PM).
Template
- AWS provide built in template for ease resource creation
- you can create your own template on web.


To visualise cloud formation template use Application composer.
