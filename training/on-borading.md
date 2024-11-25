# On Boarding New Employee

## Get access to various resources

- Stellar
    - Complete the two [Aspire](https://yarditrainingservices.yardielearning.com/) security courses \
    Login to Aspire and assign following courses to the new employee through Supervisor mode.
        - CST 010 - Supporting Hosted Clients
        - NE 100 - Security Awareness
    - Once courses are completed, download the transcript of the user courses.
    - Raise a stellar request \
    Initial Stellar Access can be requested via Cloud Request > New user setup case logged under PIN 100052397
    - Attach courses transcript to the stellar request.
    ```mermaid
    flowchart LR
    A[Start] --> B[Assign Security Courses]
    B --> C{Course Complete?}
    C --> |Yes| E[Download Transcript]
    C --> |No| F[Send Reminder]
    F --> C
    E --> G[Add Stellar Request]
    G --> I[Attach transcripts]
    I --> J[End]

    ```
- yCRM
- TFS
    - In n yCRM, navigate to Tracking Request > Source Control > Source Control Access Request.
    - In the Source Folder field, enter the path to the folder.
- WeWork
- New Horizon VM - Create a separate IT Ticket.
- MySQL databases
    - Local DB - Prakash to create new user
    - QA - Add stellar request
- Duo Mobile
- Chat IQ Admin - Dev, QA (CrmIQ, FlexQA)



## MySQL Databases

| Env        | IP            | Database    |Username       |Password    |
|------------|---------------|-------------|---------------|------------|
|QA          |10.168.212.63  |omni_qa_db   |               |            |
|Prod        |10.168.212.43  |omni_prod_db |               |            |
|Daily       |10.168.212.65  |             |               |            |
|UK          |               |             |               |            |
|Report qa   |10.97.212.41   |omni_qa_db   |<ysi username> |            |
|Report prod |10.97.212.40   |omni_prod_db |               |            |
|Local DB    |pcz218dbl23    |omni_qa_db   |prakashd       |TLzWqu8Kyp  |


## Training Schedule

TFS location for training material: $/Underdevelopment/SiddharthMehta

| Technology       | Date  | Point of Contact | Traning details                             |
|------------------|-------|------------------|---------------------------------------------|
| Web Introduction | Day 1 | TL/Mgr           | [TFS]/Training/Web introduction.mp4 |
| HTML/CSS         | Day 2 | TL/Mgr           | [Online Tutorial](http://www.w3schools.com/html/) |
| Javascript       | Day 3 | TL/Mgr           | [Online Tutorial](http://www.w3schools.com/js/) |
| Typescript       | Day 4 | TL/Mgr           | [Online Tutorial](https://www.w3schools.com/typescript/) |
| C#               | Day 5 | TL/Mgr           | [Online Tutorial](https://www.w3schools.com/cs/index.php) |
| Angular          | Day 6 | TL/Mgr           | [TFS]/AngularCafe/A16/Trainings/SQLServer/Day 1 - Setup and Introduction to Elevate |
|                  | Day 7 | TL/Mgr           | Project Structure                           |
|                  | Day 8 | TL/Mgr           | Basic Angular Controls                      |
|                  | Day 9 | TL/Mgr           | Reports and Dashboards                      |
|                  | Day 10| TL/Mgr           | Element Security and Shipyard deployment    |

