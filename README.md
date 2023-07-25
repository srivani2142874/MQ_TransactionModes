# MQ_TransactionModes
Checking the behaviour of MQ output node during unhandled exceptions. 
Understand the Transaction mode
IF TM IS YES-- It goes to backout queue defined on queue level
               if there is no backout  queue it will go to Dead Letter Queue on queue manager level
               if no dead letter queue found it might be in infinite loop
IF TM IS NO--   the message in queue will be lost
IF TM IS AUTOMATIC & NOT PERSISTENT-- ACT AS NO MODE
IF TM IS AUTOMATIC & PERSISTENT --ACT AS YES MODE
Integration Server-- MQ_TM_SERVER
Queue-PRACTICEQUEUE

IMAGES OF MESSAGE FLOW AND OUTPUT
(https://github.com/srivani2142874/MQ_TransactionModes/assets/140478553/350485e1-bd27-48b8-98b3-f627a09aee5f)
(https://github.com/srivani2142874/MQ_TransactionModes/assets/140478553/ac69457f-a58c-4dd0-982b-e99a7f9432d0)


