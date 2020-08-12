# automatedTAM
A power automate for TAM's

Reactive email sort:

There are 3 versions for whoever is interested in trying these out.
They all require some minimal configuration to work on your specific outlook folders.
I have marked the sections that require configuration and am happy to walk anyone through the configuration.

Step 1: Download the zip file
Step 2: Go to https://www.office.com/ -> Power Automate -> My Flows
Step 3: Click the Import button and select the downloaded file
Step 4: During import connectors will be setup – (This has recently changed so I can’t specify exactly how you need to proceed here) as I import these into my existing environment likely you will need to specify ‘create new connectors’
Step 5: Edit the flow to Configure the options as required


1.	Simple email sort – Determine that the email is a reactive case and move to a reactive folder
https://github.com/jasondb1/automatedTAM/raw/master/ProcessCustomerEmails_v1.0.3_basic.zip

Functionalities:
Classifies email as reactive
Moves reactive emails to reactive folder

Requires configuring the reactive email folder


2.	Process Customer Emails – Determine that the email is a reactive case and move to a reactive folder or a general folder

Functionalities:
Classifies email as reactive / non-reactive
Moves email to customer main mail box or reactive mailbox
Classifies and moves backup accounts to a backup reactive folder

https://github.com/jasondb1/automatedTAM/raw/master/ProcessCustomerEmails_v1.0.3_standard.zip


Requires:
outlook folder structure that sets up each customer
configuring the reactive/general customer email folders, criteria for identifying customers

Here is my structure:
Omitted for privacy
 



3.	Process Customer Emails – with Critsit options 
https://github.com/jasondb1/automatedTAM/raw/master/ProcessCustomerEmails_v1.0.3_with_critsit.zip

Functionalities:
Classifies email as reactive / non-reactive
Moves email to customer main mail box or reactive mailbox
Classifies and moves backup accounts to a backup reactive folder

Teams Integration - 
Detect Critsit and post option card to teams – flowbot – can add to planner/todo, open case or ping im

Requires:
A teams channel (personal channel used)
configuring the reactive/general customer email folders, criteria for identifying customers,
