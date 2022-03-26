# Project4EC530

## Phase 2: Simple queue system using Celery and rabbitmq server
1. Start rabbit server using command sudo rabbitmq-server
2. To see processes in action: celery -A queueSystem worker -l INFO 
3. In python interactive shell run:<br>
from queueSystem import txt2speech<br>
for i in range(0,1000):<br>
  txt2speech.delay()
