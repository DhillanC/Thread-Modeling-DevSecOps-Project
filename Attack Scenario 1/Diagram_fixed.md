```mermaid

flowchart LR





    A[GitHub Repos] --> B{CI/CD Pipeline GH Actions}

    A[Reconnaissance] -->|Identify target| B

    B[Reconnaissance] -->|Gather information| B

    B[Weaponization] -->|Craft malicious payload| D

    D[Delivery] -->|Send phishing email| D

    D[Delivery] -->|Trick user to download payload| D

    D[Exploitation] -->|Execute payload| D

    D[Exploitation] -->|Gain access to web server| H

    H[Installation] -->|Install backdoor| H

    H[Installation] -->|Establish persistence| H

    H[Command and Control] -->|Communicate with C&C server| H

    H[Command and Control] -->|Issue commands| L

    H[Actions on Objectives] -->|Steal sensitive data| M