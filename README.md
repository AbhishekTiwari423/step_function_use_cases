# step_function_use_cases
Various step function use cases
Use Caes#
1. Step function to execute Glue job from lambda
  -> CloudWatch/Event triggeres step function.
  -> Lambda function is invoked.
  -> Lambda function completed basic checks and generates parameters required for Glue job execution.
  -> If Glue job fails, SNS notification is triggerd to inform stakeholders.
  -> NO notification is send in case Glue JOb is sucessfull.
  -> Joob gets completed.
