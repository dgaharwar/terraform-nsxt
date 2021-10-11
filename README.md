# terraform-nsxt
very simple, and single flat tf file to get NSX-T configured with a sample T1 router and associated logical segments and DFW policy

Step1: 
install terraform on your chosen linux box
in the same dir as the main.tf file

Step2:
Initialise the requried NSX-T provider
  terraform init

Step3:
Validate the plan
  terraform plan 
  
Step4:
Execute the plan
  terraform apply 
  
Step5:
Delete the plan
  terraform destroy
  
NOTE:
Be sure to check in the manager portion of the NSX-T UI, as pre NSX-T 3.2, TF uses the management API (not the policy API).
In time, Policy API (and UI) will show the TF created objects
